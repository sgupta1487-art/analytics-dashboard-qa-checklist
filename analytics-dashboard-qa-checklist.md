# Analytics Dashboard QA Checklist

A practical checklist to validate analytics dashboards before sharing with stakeholders or releasing to production.

---

## 1. Data Source Validation
- [ ] Data source connections are correct and point to the expected environment (dev / test / prod)
- [ ] Data refresh schedule is confirmed and documented
- [ ] No broken queries or failed refreshes
- [ ] Row counts match source system expectations

---

## 2. Data Accuracy & Calculations
- [ ] Key metrics match source data or validated reports
- [ ] Aggregations (sum, average, count, distinct count) are correct
- [ ] Time-based calculations (YTD, MoM, YoY) are accurate
- [ ] Null, zero, and negative values are handled correctly
- [ ] Currency, units, and rounding are consistent

---

## 3. Filters, Slicers & Drill-Downs
- [ ] All filters return expected results
- [ ] Default filter values are correct
- [ ] Filter combinations do not break visuals
- [ ] Drill-down and drill-through functionality works as expected
- [ ] Filters reset properly when cleared

---

## 4. Performance & Load Testing
- [ ] Dashboard loads within acceptable time limits
- [ ] Visuals render without timeouts or errors
- [ ] Performance tested with large data volumes
- [ ] Unused fields or visuals are removed

---

## 5. Usability & Clarity
- [ ] Dashboard purpose is clear within 10 seconds
- [ ] Metric definitions are understandable to non-technical users
- [ ] Titles, labels, and tooltips are clear and accurate
- [ ] No overlapping visuals or truncated text
- [ ] Consistent formatting across pages

---

## 6. Security & Access Control
- [ ] Row-level or column-level security is validated
- [ ] Sensitive data is masked or excluded
- [ ] User access matches role expectations

---

## 7. Edge Cases & Validation
- [ ] Dashboard behaves correctly with no data
- [ ] Dashboard behaves correctly with single-record scenarios
- [ ] Date ranges at boundaries are handled correctly
- [ ] Historical data does not change unexpectedly

---

## 8. Final Review & Sign-Off
- [ ] Stakeholder review completed
- [ ] Known limitations are documented
- [ ] QA sign-off completed
- [ ] Deployment readiness confirmed
