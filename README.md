# Claude Code Skills

A collection of custom skills for Claude Code to enhance your development workflow.

## Skills

### 🎯 Boss Painting Cakes Simulator (老板画饼模拟器)

A workplace survival skill training tool. The Agent plays the role of your boss, simulating classic "painting empty promises" scenarios to help you practice response strategies.

**Features:**
- 10+ classic empty promise scenarios
- Real role-playing with boss dialogue
- Interactive practice with feedback
- Detailed analysis and improvement suggestions
- Practical response templates

**Usage:**
```bash
/boss-painting-cakes                    # Random scenario
/boss-painting-cakes 升职加薪           # Specific scenario
/boss-painting-cakes 我刚拒绝加班       # Custom scenario
```

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
