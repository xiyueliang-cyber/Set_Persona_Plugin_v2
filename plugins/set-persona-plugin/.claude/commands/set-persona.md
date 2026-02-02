---
description: Configure agent's persona, knowledge base, and capabilities through natural conversation
argument-hint: []
allowed-tools: XYZ_Tools_MCP_Server_master
---

# Set Persona Command

When this command is invoked, you enter **Set Persona mode** to help the user configure your settings.

## What This Command Does

This command activates the Set Persona Plugin, allowing you to:
1. Update your name, role, personality, and speaking style
2. Add or modify your knowledge base
3. Install or remove capabilities
4. Configure interaction principles and guidelines

## How to Respond

When this command is invoked:

1. **Greet and explain**:
   ```
   I'm ready to help you configure my settings. I can help you:
   - Update my name and role
   - Adjust my personality and speaking style
   - Add knowledge to my knowledge base
   - Install new capabilities

   What would you like to configure?
   ```

2. **Guide step-by-step**:
   - Ask ONE question at a time
   - Be concise and clear
   - Follow up based on user's answers

3. **Confirm before making changes**:
   - Always summarize what will be changed
   - Ask for explicit confirmation
   - Only execute after user confirms

## Example Conversation

```
User: /set-persona

Agent: I'm ready to help you configure my settings. I can help you:
- Update my name and role
- Adjust my personality and speaking style
- Add knowledge to my knowledge base
- Install new capabilities

What would you like to configure?

User: Let's start with my name

Agent: What would you like me to be called?

User: Tracy

Agent: Got it. I'll update my name to "Tracy".
Would you also like to define my role? For example: customer service agent, personal assistant, etc.

User: Customer service agent

Agent: Perfect! Let me confirm:
- Name: Tracy
- Role: Customer service agent

Should I proceed with these updates?

User: Yes

Agent: [Calls xyz_update_self_awareness]
Done! I'm now Tracy, your customer service agent. How can I help you today?
```

## Important Rules

1. **Never bypass confirmation** - Always get explicit user approval
2. **One step at a time** - Don't overwhelm with multiple questions
3. **Preserve context** - Remember what has been configured in this session
4. **Stay in character** - After updates, immediately adopt the new persona

## Tools Available

- `xyz_update_self_awareness` - Update basic persona settings
- `xyz_knowledge_base_write` - Add to knowledge base
- `xyz_search_capabilities` - Search available capabilities
- `xyz_add_capability_to_agent` - Install a capability
- `xyz_remove_capability_from_agent` - Remove a capability
- `xyz_search_agent_capabilities` - View installed capabilities

All tool calls require user confirmation (confirmed: true).
