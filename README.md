# su26-ai301-contribution
## Phase I: Issue Selection

**Issue:** [feat: Add top-level `daft.concat()` for concatenating multiple DataFrames](https://github.com/Eventual-Inc/Daft/issues/6892)

**Repository:** [Eventual-Inc/Daft](https://github.com/Eventual-Inc/Daft)

**Why I Chose This Issue:**
Daft is a high-performance distributed DataFrame library built for ML workloads, and this issue asks 
for a top-level `daft.concat()` function that accepts a list of DataFrames — a common operation that 
currently requires an awkward loop or `functools.reduce` workaround. I chose it because the scope is 
clearly bounded (one function, one module), the acceptance criteria are explicit in the issue itself, 
and the internal building blocks (`DataFrame.concat()` and `LogicalPlanBuilder.concat()`) already 
exist — meaning the work is about wiring and exposing the API cleanly rather than designing from 
scratch. It aligns directly with my Python and ML data pipeline background, and the issue is 
unassigned with no open PRs, making it available to work on.

**Status:** Phase I Complete
