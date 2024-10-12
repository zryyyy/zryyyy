### References

- [中文文案排版指北](https://github.com/sparanoid/chinese-copywriting-guidelines/blob/master/README.zh-Hans.md)
- [rzashakeri/beautify-github-profile](https://github.com/rzashakeri/beautify-github-profile)
- [Skill Icons](https://skillicons.dev)
- [microsoft/fluentui-emoji-animated](https://github.com/microsoft/fluentui-emoji-animated)
- [Tarikul-Islam-Anik/Animated-Fluent-Emojis](https://github.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis)

### Develop

```bash
LAST_USER_COMMIT=$(git log --pretty=format:'%H %an' | grep -Ev 'readme-bot|github-actions\[bot\]' | head -n1 | awk '{print $1}')

echo "Last user commit: $LAST_USER_COMMIT"

git reset --hard $LAST_USER_COMMIT

git rebase -i --root
```
