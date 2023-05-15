# cognitive-agent

Hoping to make a cognitive agent.

## Initial Plan

- Use [AutoGPTQ](https://github.com/PanQiWei/AutoGPTQ) for GPU accelerated 4-bit inference.
- Implement custom [LangChain](https://github.com/hwchase17/langchain) wrappers for anything that isn't supported.
  - Notably, LangChain's [HuggingFacePipeline](https://python.langchain.com/en/latest/reference/modules/llms.html#langchain.llms.HuggingFacePipeline) wrapper is poorly implemented (i.e., hardcoded to 2 tasks).
  - Wrapper above doesn't actually do much, easier to just create custom wrappers.
- Peruse of LangChain's wide variety of other self-hosted libraries support (namely memory systems).
  - Intending to implement own Graph Knowledge Base system eventually.
