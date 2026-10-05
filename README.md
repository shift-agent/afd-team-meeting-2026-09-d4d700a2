# AFD Team Meeting Sept 2026 deck (local prep, NOT published)
Contents: index.html (18 slides, noindex meta added), assets/ (4 relative images), PDF download copy.
Prior pattern: shift-agent/afd-consistency-training (public, Pages from main root, legacy build, no CNAME).
Publish steps (run only on Glenn's "publish the AFD deck"):
1. cd this folder; git init -b main; git add -A; git commit -m "AFD team meeting deck"
2. gh repo create shift-agent/afd-team-meeting-2026-09 --public --source=. --push
   (private repos need a paid plan for private Pages)
3. gh api -X POST repos/shift-agent/afd-team-meeting-2026-09/pages -f 'source[branch]=main' -f 'source[path]=/'
4. URL: https://shift-agent.github.io/afd-team-meeting-2026-09/ (builds in ~1 min)
