# Open Questions and Validation Points

## Decisions Needed Before the Hackathon

- Will the demo be a software-only plush simulation, or will it connect to real hardware such as a development board, XiaoZhi board, microphone, or camera?
- Which voice pipeline will be used: browser recording plus cloud model, mobile recording, or hardware button trigger?
- Which growth metaphor should be chosen: memory leaves, shared story tree, companion level, or interest map?
- Will there be a parent view? If yes, should it be a summary panel, message-style prompt, or family story card?
- How large should the English learning component be: the main feature, or a lightweight element inside companionship stories?

## Product Definition Questions

- What exactly is the plush's role: friend, pet, classmate, learning buddy, family recorder, or the child's little counterpart?
- What is its relationship with parents: helping parents understand the child, or helping the child express themselves to parents?
- How proactive should it be: asking once a day, or triggered by events?
- How should "co-growth" appear: more memories, personality changes, story progress, ability upgrades, or visible rituals?
- Does it need eyes, expressions, lights, or motion, or should the hackathon only use voice and screen-based expression?

## Technical Validation Points

- Will speech recognition latency break the feeling of companionship?
- Is the TTS voice child-friendly enough?
- Is memory retrieval stable, and can it accurately reference what the child said before?
- How can the system avoid fabricating memories about the child?
- How should negative emotion, safety-sensitive content, and private content be handled?

## Business and Compliance Validation Points

- What are the compliance boundaries for child-facing large-model products in the target market?
- How should the product be described in a China demo to avoid implying it is a launch-ready child-facing large-model hardware product?
- If going overseas, should the target market be North America, Southeast Asia, or Chinese-speaking families overseas?
- How much would parents pay for the hardware, and would they accept a subscription?
- Should the IP be self-owned, partner-based, or a neutral original character first?

## Post-Hackathon Extensions

- Multi-agent community: each child's plush agent interacts with other children's plush agents.
- Parent-child co-creation: the plush turns child-parent conversations into storybooks.
- Long-term memory system: child growth trajectory, interest changes, and language ability changes.
- Family memoir: extend from child companionship to family memory, elderly companionship, and intergenerational communication.
- Hardware ecosystem: standardized interfaces, open-source shells, and combinations of plush/IP/sensors.

## Current Recommendation

For the hackathon, choose the smallest complete loop: voice conversation + lightweight memory + one growth visualization + parent summary. Keep multi-agent community, subscription monetization, hardware mass production, and full compliance systems at the vision layer so they do not consume the demo.
