Rule of Supporting
==============================
Mindset
------
1. Accept that your productivity will be killed for the week
2. Stay focused on the suport chat and your emails
3. Keep you are reachable and respond to support ASAP 
4. Notify support when you will be away for a long time or find a backup
5. Communicate using compliant tool


Flow
----
![[Flow to resolve Prod Issue.excalidraw]]
```mermaid
flowchart TD

st((Start))
e((end))
what(What happened
any impact & deadline)
preCheck{Support analysis 
& action}
back((push back and 
challenge support))
ticket{support raise ticket}
ca(check alone at first)
rc(Call someone help 
to find out root cause)
fresh(involve freshman)
2w(Figure out root cause
When & Why it happened)
cond{Issue?}
fix(Provide fix plan &
 update deadline) 
update(Update impact scope
and deadline)
UAT(Test solution in UAT)
confl(Record and update guaide
in confluence)
ai(Enhance develop/release 
flow to avoid issue)
aa(Avoid alert)

st-->what--> preCheck
preCheck --no --> back
preCheck --yes--> ticket --no --> back
ticket --yes--> fix
what-->ca -->rc --> fresh --> 2w
ca -->2w-->cond
cond-- yes -->update--> UAT -->fix -->confl --> ai-->e
cond-- no --> aa--->e
```
