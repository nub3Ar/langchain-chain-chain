# Teaching chatGPT to write langchain code, written with langchain


Being consistent with my vision that execution should be zero marginal cost in the future, I was bothered when chatGPT couldn't write langchain code.

So I fed a langchain one-pager into chatGPT, \
which generated the langchain code, \
which can be fed more langchain documentation, \
which can generate more langchain code. \
Life is beautiful again

Written at 2AM, but serious takeaways:

1. With the best LLMs being mostly frozen, prompt is still the best way to alter model states. ChatGPT’s 1-shot learning ability is much more impressive than I thought.
2. Ideally, these information should be encoded through fine-tuning (like what CoPilot/CodeComplete probably did) or adapters (e.g. LoRA) on proprietary codebases, but for any new codebase, a “codebase card” is probably the fastest way to solve the cold start problem
3. I am deliberately creating things that don't scale to demonstrate ideas. If I want to scale, I need to make friends with really good data/infra/backend engineers because that’s the part I cannot bother to learn (Daniel said he is too busy for my bs)