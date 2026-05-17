# Claude Code Skills

A collection of custom skills for Claude Code to enhance your development workflow.

## Skills

### 🎯 Boss Painting Cakes Simulator (老板画饼模拟器)

A workplace survival skill training tool with **interactive dialogue system**. The Agent plays the role of your boss, simulating classic "painting empty promises" scenarios.

**Features:**
- 10+ classic empty promise scenarios
- **Interactive choice system** - Choose from A/B/C/D options or type freely
- **Multi-turn dialogue** - Boss responds and escalates based on your choices
- **Dynamic boss personality** - Tactics evolve based on conversation
- **Scene switching** - Change scenarios mid-conversation
- Detailed analysis and improvement suggestions

**Usage:**
```bash
/boss-painting-cakes                    # Enter main menu, choose scenario
/boss-painting-cakes 升职加薪           # Direct to specific scenario
```

**How it works:**
- Start from main menu, choose a scenario (1-10) or describe custom scenario
- Each round: Boss speaks → You choose A/B/C/D or type freely
- Boss adapts based on your response (escalates, softens, changes topic)
- Use commands: [继续] [换话题] [施压] [温和] [结束] [换场景]
- End with "结束" or "复盘" for detailed analysis

**Scenarios included:**
1. Promotion promises
2. Stock option temptation
3. Unpaid overtime
4. IPO promises
5. Team building instead of raises
6. "Young people should learn"
7. Project success rewards
8. Industry future promises
9. Emotional manipulation
10. Comparison with other companies

**Installation:**
```bash
# Clone the repository
git clone https://github.com/ZW1-ing/-skill.git

# Copy to Claude Code skills directory
cp -r -skill/boss-painting-cakes ~/.claude/skills/
```

**Configuration:**
Add to `~/.claude/settings.json`:
```json
{
  "skills": [
    {
      "name": "boss-painting-cakes",
      "path": "~/.claude/skills/boss-painting-cakes/skills/boss-painting-cakes/SKILL.md",
      "enabled": true
    }
  ]
}
```

## File Structure

```
skills/
├── .gitignore
├── README.md
└── boss-painting-cakes/
    ├── .claude-plugin/
    │   └── plugin.json
    ├── skills/
    │   └── boss-painting-cakes/
    │       ├── SKILL.md
    │       └── references/
    │           ├── classic-phrases.md
    │           └── communication-tips.md
    └── README.md
```

## Contributing

Feel free to add more skills or improve existing ones. Each skill should follow the Claude Code skill format:

1. Create a directory for your skill
2. Add a `SKILL.md` file with proper frontmatter
3. Include any reference materials in a `references/` directory
4. Update this README with documentation

## License

MIT License

## Author

- **ZW1-ing** - [GitHub Profile](https://github.com/ZW1-ing)

## Acknowledgments

- Thanks to the Claude Code team for the skill system
- Inspired by real-world workplace scenarios
- Built for learning and practice purposes
