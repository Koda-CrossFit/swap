# Koda Iron Games 2026: Born Primitive Swap

Check-in page where athletes ask to trade their Born Primitive kit pieces (sports bra and/or shorts) for a different size or style.

- Live: https://koda-crossfit.github.io/swap/
- Backend: `bpSwapRequest` action in the Koda coaching Apps Script (`koda-coaching/apps-script/Code.js`)
- Sheet: "Koda Iron Games 2026 - Born Primitive Swap Requests" (GET `?action=bpSwapInfo` returns the URL)

Each submission writes one row per item. A new row is matched against every open row of the same item where each person has what the other wants ("Any style" on the wants side matches any style). Both rows get a "Possible Match" note and turn green, and Kevin gets an email. Set Status to Swapped or Cancelled to take a row out of matching.

Style names in `index.html` (ITEMS) must match `BP_SWAP_STYLES` in Code.js.
