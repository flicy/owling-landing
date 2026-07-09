# Hackathon Execution Spec

## Demo Goal

In 3-5 minutes, help the audience understand: this is an AI companion plush prototype that remembers the child, proactively talks with the child, and grows together with the child.

## Recommended Demo Script

1. The child wakes the plush for the first time and tells it their name, favorite things, and today's English theme.
2. The plush responds in a warm, child-friendly tone and invites the child to tell one thing that happened today.
3. The child shares a simple event, such as drawing a blue dinosaur, arguing with dad, or wanting to learn how to say "I feel a little nervous."
4. The plush turns the event into a "memory leaf" or part of a "shared story tree."
5. In a second conversation, the plush references that memory: "Would the blue dinosaur you drew yesterday like to learn a new word today?"
6. A parent view or display panel shows a summary: the child's interests, emotions, English expression, and topics to continue discussing.

## MVP Feature List

- Voice input: browser recording, mobile recording, or a simulated hardware button.
- Voice output: TTS or preset voice; continuity matters more than audio sophistication.
- Conversation agent: proactively asks questions, responds to the child, and keeps a child-friendly tone.
- Memory storage: local JSON, SQLite, or a simple database.
- Memory retrieval: the next conversation must reference a previous turn or previous session.
- Growth visualization: choose one of memory leaves, story tree, companion level, or interest map.
- Parent summary: at least a text summary; no need for a full parent app.

## Suggested Memory Data Structure

```json
{
  "child_profile": {
    "name": "Mia",
    "age": 7,
    "interests": ["dinosaurs", "drawing"],
    "family_members": ["mom", "dad"]
  },
  "short_term_events": [
    {
      "date": "2026-07-09",
      "event": "Drew a blue dinosaur",
      "emotion": "excited",
      "english_phrase": "blue dinosaur",
      "follow_up_prompt": "Ask about the dinosaur's adventure tomorrow."
    }
  ],
  "growth_state": {
    "companion_level": 2,
    "memory_leaves": 5,
    "current_story": "The Blue Dinosaur Learns English"
  }
}
```

## Plush Personality

- Proactive but not intrusive.
- Like a friend and a gentle family recorder.
- Does not replace parents and does not imitate adult intimacy.
- When negative emotions appear, first receive the feeling, then encourage the child to communicate with parents.
- Keeps English learning lightweight, playful, and low-pressure.

## Visualization Suggestions

Choose one metaphor first; do not implement too many at once:

- Memory leaves: each daily conversation creates one leaf.
- Shared story tree: the story written by the child and plush grows into a tree.
- Companion level: the plush levels up through companionship, but avoid manipulative monetization.
- Interest map: shows themes the child mentions repeatedly.

## What Not to Build for the Hackathon

- Do not build a full child social platform.
- Do not build complex multi-agent battles, recharge systems, or HP-loss mechanics.
- Do not build a real mass-production hardware plan.
- Do not spend most of the time on shell design or PCB work unless hardware is already available.
- Do not turn the product into a pure English drill tool.
- Do not introduce an uncontrolled open chat community in a child-facing scenario.

## Differentiation Judges Can Understand

A normal AI toy answers a child's questions; this plush remembers the child's life and grows with the child.

A normal English learning product emphasizes practice efficiency; this product places English inside the child's own stories, emotions, and family relationships.

A normal hardware device is a terminal; this plush is a relationship interface between the child, parents, physical plush, and cloud agent.
