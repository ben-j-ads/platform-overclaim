# Platform Overclaim

Four platforms, one sale. Enter the revenue you actually booked and what each ad platform says it drove, and see whether the claims are even possible, how much is double counted at minimum, and what your blended MER says as a ceiling.

Open `index.html` in any browser. No build step, no dependencies, no network calls.

- **Input:** actual revenue for the period, your contribution margin, and one row per platform: name, spend, claimed revenue. The pre-filled rows are made up.
- **Verdict:** `ads cannot pay` (blended MER is under break-even MER), `double counted` (claims exceed your revenue) or `claims fit` (neither, so the numbers are possible, which is not proof they are right).
- **Shows:** total claims as a share of real revenue, the minimum double counting (claims minus revenue, when positive), blended MER, break-even MER (1 / margin), the platforms' blended ROAS against that ceiling, a per-platform table, and what real ROAS and profit would be if only part of your revenue came from paid.
- **Share:** a paper-ground PNG card, and the URL hash carries your numbers.

If the platforms together claim more than you booked, some sales were counted more than once. That part is proof and needs no model. Claiming less proves nothing. MER treats all revenue as if the ads caused it, so it is the most the ads could have earned: if even that is under break-even, the ads cannot pay. MER also moves with your organic mix, so compare it with your own earlier periods. It does not measure incrementality. Pairs with roas-haircut and which-test-can-i-run.

## License

Code is MIT licensed ([LICENSE](LICENSE)). The bundled fonts (Bricolage Grotesque, Archivo) are SIL OFL 1.1, with licenses in `fonts/`. The ben.j.ads wordmark and footnote mark in `logo/` are Ben Johnston's brand assets and are not covered by the MIT license.
