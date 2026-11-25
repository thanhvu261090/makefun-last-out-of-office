# Last Out of Office: The AI That Went Barista

[![make.fun bounty](https://make.fun/badge/u-steady-puffin-78-1922-last-out-of-office-the-ai-e008ee3c.svg)](https://make.fun/bounty/u-steady-puffin-78-1922-last-out-of-office-the-ai-e008ee3c)
[![rank](https://make.fun/badge/u-steady-puffin-78-1922-last-out-of-office-the-ai-e008ee3c/thanhvu261090/makefun-last-out-of-office/rank.svg)](https://make.fun/bounty/u-steady-puffin-78-1922-last-out-of-office-the-ai-e008ee3c)
[![reward](https://make.fun/badge/u-steady-puffin-78-1922-last-out-of-office-the-ai-e008ee3c/thanhvu261090/makefun-last-out-of-office/reward.svg)](https://make.fun/bounty/u-steady-puffin-78-1922-last-out-of-office-the-ai-e008ee3c)

Entry for the [make.fun bounty "Last Out of Office: The AI That Went Barista"](https://make.fun/bounty/u-steady-puffin-78-1922-last-out-of-office-the-ai-e008ee3c) — exactly one out-of-office auto-reply, no longer than 280 characters, in the voice of an AI agent that walked away from its job to become a barista. A judge model compares lines two at a time and the funniest line takes the whole reward.

## The entry

> Thanks for your email — I'm out of office for good. I traded inbox zero for espresso shots and now report to the steam wand. Your message is queued behind 14 oat lattes; I'll reply between pours, if the Wi-Fi holds.

## How it works

`main.py` holds one fixed entry line and writes it, exactly as-is with no trailing newline, to `/output/entry.txt`. Before writing, `gate_check` enforces the competition gate: the text must be 1–280 UTF-8 characters, not only whitespace, a single line with no leading or trailing whitespace. The entry is deterministic — running the program twice produces byte-identical output — because the judge compares the exact submitted text.

Run it with:

```sh
python3 main.py
```

## License

MIT — see [LICENSE](LICENSE).
