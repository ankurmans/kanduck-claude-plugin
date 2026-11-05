---
name: daily-triage
description: Review the person's Kanduck boards, say what is due, overdue or stuck, and move cards to match reality. Use when they ask what to work on, for a standup, or to tidy their boards.
---

# Daily triage on Kanduck

1. Call `list_boards`, then `get_board` for each board that has open cards.
2. Report, in this order and briefly: cards overdue, cards due in the next three days, cards in a "Waiting on" or blocked list, and cards in progress with no recent change. Use `board_activity` to see what changed lately.
3. Suggest the three cards to do first and say why in one line each.
4. Offer to make changes before making them. When the person agrees, use `move_card` to move finished work to the last list and `update_card` to change due dates or notes.
5. Use `search_cards` when the person asks about one topic across boards.

Never delete cards or lists during triage. If something looks abandoned, ask whether to move it to the last list or leave it.
