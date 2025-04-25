# Agent Comparison

| Feature                          | LangGraph | Agents SDK | Google ADK | LangChain | AutoGen | CrewAI | Agno | Temporal | Smol Agents | LlamaIndex | DSPy | Pydantic AI | Letta | Mastra |
| -------------------------------- | --------- | ---------- | ---------- | --------- | ------- | ------ | ---- | -------- | ----------- | ---------- | ---- | ----------- | ----- | ------ |
| Workflow orchestration Framework | [x]       | [ ]        | [ ]        | [ ]       | [x]     | [!]    | [ ]  | [x]      | [ ]         | [x]        | [x]  | [!]         | [ ]   | [x]    |
| Agent Abstractions               | [x]       | [x]        | [x]        | [x]       | [x]     | [x]    | [x]  | [ ]      | [x]         | [x]        | [x]  | [x]         | [x]   | [x]    |
| Multi Agent Abstractions         | [x]       | [x]        | [x]        | [ ]       | [x]     | [x]    | [x]  | [ ]      | [ ]         | [x]        | [ ]  | [ ]         | [x]   | [!]    |
| Declarative API                  | [x]       | [?]        | [?]        | [?]       | [x]     | [x]    | [?]  | [ ]      | [?]         | [x]        | [ ]  | [x]         | [?]   | [x]    |
| Imperative API                   | [!]       | [?]        | [?]        | [?]       | [ ]     | [ ]    | [?]  | [x]      | [?]         | [ ]        | [x]  | [ ]         | [?]   | [ ]    |
| Short term memory storage        | [x]       | [ ]        | [x]        | [x]       | [x]     | [x]    | [x]  | [ ]      | [ ]         | [x]        | [ ]  | [ ]         | [x]   | [x]    |
| Long term memory storage         | [x]       | [ ]        | [x]        | [ ]       | [x]     | [x]    | [x]  | [ ]      | [ ]         | [ ]        | [ ]  | [ ]         | [x]   | [x]    |
| Human in the loop                | [x]       | [ ]        | [ ]        | [ ]       | [ ]     | [ ]    | [ ]  | [!]      | [ ]         | [x]        | [ ]  | [ ]         | [ ]   | [x]    |
| Human on the loop                | [x]       | [ ]        | [ ]        | [ ]       | [ ]     | [ ]    | [ ]  | [ ]      | [ ]         | [x]        | [ ]  | [ ]         | [ ]   | [ ]    |
| Streaming                        | [x]       | [x]        | [x]        | [x]       | [x]     | [x]    | [x]  | [ ]      | [ ]         | [x]        | [ ]  | [x]         | [x]   | [x]    |
| Optimization                     | [ ]       | [ ]        | [ ]        | [ ]       | [ ]     | [ ]    | [ ]  | [ ]      | [ ]         | [ ]        | [x]  | [ ]         | [ ]   | [ ]    |
| Code interpreter                 | [ ]       | [x]        | [x]        | [ ]       | [x]     | [x]    | [ ]  | [ ]      | [x]         | [ ]        | [ ]  | [x]         | [ ]   | [ ]    |
| Tracing                          | [x]       | [x]        | [ ]        | [x]       | [ ]     | [ ]    | [ ]  | [ ]      | [ ]         | [ ]        | [ ]  | [x]         | [ ]   | [ ]    |
| Studio                           | [x]       | [ ]        | [x]        | [x]       | [x]     | [ ]    | [x]  | [ ]      | [ ]         | [ ]        | [ ]  | [ ]         | [x]   | [x]    |
| Low code builder                 | [ ]       | [ ]        | [ ]        | [ ]       | [x]     | [x]    | [ ]  | [ ]      | [ ]         | [ ]        | [ ]  | [ ]         | [x]   | [ ]    |
| Prescribed project setup         | [!]       | [ ]        | [x]        | [ ]       | [ ]     | [x]    | [ ]  | [ ]      | [ ]         | [!]        | [ ]  | [ ]         | [ ]   | [x]    |
| Fault tolerance                  | [x]       | [?]        | [?]        | [?]       | [ ]     | [ ]    | [?]  | [x]      | [?]         | [x]        | [?]  | [ ]         | [?]   | [ ]    |

- `[x]` means it has it
- `[ ]` means it doesn't have it
- `[?]` means it has it but it's not clear how good it is
- `[!]` means it technically has it but isn't very good or isn't super agent specific or isn't the primary recommended way
- "Human in the loop" refers to things besides chat (eg review/approve tool calls)
- "Human on the loop" refers to time travel like functionality
- "Code interpreter" is checked if the authors of the framework also implement a code interpreter
- "Tracing" is checked if the authors of the framework also implement an LLM/agent specific tracing platform
