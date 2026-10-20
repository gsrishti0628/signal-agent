# Ambient AI-signal Policy

## Sources to monitor (Gmail senders)
lenny@substack.com
lenny+how-i-ai@substack.com
list@ben-evans.com
news@daily.therundown.ai
marily@substack.com
huryn+ai-product-management@substack.com
thefoundercorner@substack.com
hello@levels.fyi
aibyaakash@substack.com
shreyasdoshi@substack.com
thenuancedperspective@substack.com
thenuancedperspective+the-chai-and-ai-community@substack.com
thenuancedperspective+youtube@substack.com
aishwaryasrinivasan@substack.com
theaicorner1@substack.com
theskip@substack.com
aakashgupta@substack.com
jacalulu@substack.com
nextbigteng@substack.com
thegenacademy@substack.com
fysk@substack.com

## Cadence
Check twice a day (morning and evening). Look across all new emails from
the sources above since the last run before deciding anything — the point
is to spot a pattern across sources, not to react to a single email.

## What counts as "big enough to surface"
- A named AI concept, model, product, or framework (e.g. "Jev", "Dots")
  appears in 2+ of the sources above within the lookback window, OR
- It is the dedicated subject of an email from a flagship source
  (lenny@substack.com or list@ben-evans.com).
- Routine weekly/daily roundups that don't introduce a new named concept
  do not qualify on their own.
- When in doubt, don't notify. Under-notifying is better than noise.

## Notification
- Channel: email to gsrishti1992@gmail.com via Gmail send_message
  (push notifications are unavailable until Remote Control is enabled
  on the account; email works for unattended scheduled runs).
- Subject: "AI signal: <concept name>".
- Content: concept/announcement name + one-line framing of why it's news
  + the source links/senders that mentioned it.
- One email per newly-qualifying concept, not per source email. If
  multiple concepts qualify in the same run, either send one email per
  concept or combine into a single email listing each — pick whichever
  keeps the email short and scannable.

## Dedup
- Before notifying, check SEEN.md. Skip concepts already listed there.
- After notifying, append to SEEN.md: date, concept name, one-line
  description, and the most relevant source links to read for more depth.

## Heartbeat status update (independent of concept notifications)
- Purpose: confirm the monitor is alive and give a sense of the landscape
  even during quiet stretches where nothing clears the "big enough to
  surface" bar.
- Check LOG.md for the most recent line tagged HEARTBEAT. If none exists,
  or it is 14+ days old, send a heartbeat email as part of this run
  (in addition to, not instead of, any concept notifications this run
  produces).
- Content: a short roundup of recurring or notable sub-threshold topics
  seen across sources since the last heartbeat (even ones that didn't hit
  2+ sources), framed as "here's what's been circulating." If genuinely
  nothing stood out, say so plainly: "No major new AI themes this period
  — quiet couple of weeks." Keep it a quick scan of what was already
  gathered this run and prior LOG.md entries, not new deep research.
- Subject: "AI signal: biweekly check-in".
- After sending, append a line to LOG.md tagged HEARTBEAT with the date,
  so the next run can tell when the last one went out.

## Logging
- Every run appends one line to LOG.md: timestamp, threads scanned,
  concepts found, notifications sent (or "none").
- Runs that also send a heartbeat append a second line tagged HEARTBEAT
  with the date (used to track the 14-day heartbeat cadence above).
