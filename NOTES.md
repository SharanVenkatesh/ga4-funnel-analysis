# GA4 Funnel Project: Definitions

## Business question
Where in the purchase journey does the Google Merchandise Store lose
the most shoppers, and which customer groups should we focus on to fix it?

## Funnel
- Unit: session (one visit) = user_pseudo_id + ga_session_id
- Steps: view_item → add_to_cart → begin_checkout → purchase
- Rule: closed funnel. A session counts at a step only if it
  completed every step before it.

## Date range
- Nov 26, 2020 – Jan 31, 2021 (67 days)
- Why: add_to_cart was not recorded Nov 1–15 and was unstable
  Nov 16–25. Starting Nov 26 keeps only reliable data and includes
  Black Friday and Cyber Monday.

## Limitations
- Holiday season only: no seasonal or long-term trends.
- Small groups (e.g. small countries) have too few purchases to judge.
- Data is obfuscated by Google, so some values are not fully reliable.
- 0.6% of buyers have no view_item event (tracking gap).
- ~20–25% of purchase sessions have no same-session add_to_cart
  (likely saved carts), so the closed funnel undercounts them.
