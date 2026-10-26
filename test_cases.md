# Manual Test Cases

Open `index.html` in a modern browser. Run each test and record your actual result; do not mark tests passed before running them.

| ID | Test | Steps | Expected result |
|---|---|---|---|
| TC-01 | Initial load | Open the page | Demo notice and example values appear |
| TC-02 | Generate readings | Press the generate button | Values update and a new table row appears |
| TC-03 | History limit | Generate more than eight readings | Only the latest eight remain |
| TC-04 | CSV export | Press download CSV | CSV downloads with `SIMULATED` labels |
| TC-05 | Photosynthesis disclaimer | Read note below table | States that photosynthesis rate is not directly measured |
| TC-06 | Mobile layout | Open on a phone | Cards wrap; table can scroll horizontally |
| TC-07 | Offline use | Open saved file with internet off | Dashboard still works |
