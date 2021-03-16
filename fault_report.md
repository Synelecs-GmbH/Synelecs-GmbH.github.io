## Fault Report Module

Fault Report Module consists of four parts

* Fault Report
* Fault State
* Fault Type
* Impact Type

### Configuration

#### Fault State (Closure State)

Fault State (Closure State) is the final status of the Fault report. This can be configured as needed. An example is:
* Accepted with Change Control Sheet
* Accepted without resolution
* Deferred to Site TIR
* Resolved


#### Impact Type

Impact Type refers to specific impact of the fault. This can be configured as needed. An example is:
* Hardware
* Software
* Documentation


#### Fault Category

Fault Category refers to specific category of the fault. This can be configured as needed. An example is:
* Observation
* Scope change
* Non Conformity Protocol Fault
* Non Conformity Implementation Fault

#### Fault Report

New Fault Report can be created directly from _Loopcheck_ document or from _Fault Report_ section. First write _Short Description_ of the fault and select _Fault Category_. _Fault Category_ field is multiselect fiels, so more than one category can be selected.
After this part is finished, describe the issue into _Fault Description_ filed.
Then click _**Save**_. Button on the top right corner will initiate _fault workflow_. Next, person who creates the fault has to then click _Actions_ -> _Classify_. 
Another person, usually from customer's side will continue the workflow by specifying _Fault Clasification_ as **Critical** or **Non-Critical** and then click _Actions_ -> _Submit Clasification_.
Fault initiator then continues and writes _Fault Report Analysis_, where the solution of the issue is written. Also, user has to select _Fault Impact_ indicating, which area (e.g. SW, HW, Doc) is affected. When this part is finished, fault initiator submits its solution using button _Actions_ -> _Submit Solution.
Client can then review the solution and either _Approve_ or _Reject_ the solution. If _Rejected_, workflow goes back for solution rework, otherwise solution is approved and can be implemented.
Once the solution is implemented, user fills out _Fault Report Closure_ section and selects proper _CLosure State_. After then click _Actions_ -> _Implement Solution_. Next stage of workflow is to _Verify Solution_ by other member of the team, or team leader. He can either accept by clicking _Verify Solution_ or reject by clicking _Rework Solution_.
Next stage is approval by customer. Again, customer has the option either to _Approve_ or _Reject_ and return the workflow back for rework. Once _Approved_, final stage is approval by Quality Representative. Also in this stage, both _Accept_ and _Reject_ is possible. With QSR Approval the workflow is finished.

Each workflow change will be logged into the document by logging user name and date.


