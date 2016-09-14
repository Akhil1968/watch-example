http://www.dotnettricks.com/learn/angularjs/understanding-angularjs-watch-digest-and-apply

Watch and apply example



--------- Objective 1 : Explaining $watch -------------------------------
- $watch is set on a varible 'myvar'. so that it observes changes to it.
- when User changes  variable 'myvar's value, the variable'ctr' is incremented. 




--------- Objective 2 : Explaining $apply -------------------------------
case 1: setInterval
- when variable 'ctr' is incremented by setInterval method of JS, angularJS framework misses to notice changes happeing to 'ctr' and does not update the UI.
- To make it update the UI, we need to call $apply 


case 2: $interval
- But when variable 'ctr' is incremented by $interval method of AngularJS, angularJS framework  notice changes happeing to 'ctr' and automatically updates the UI.
- $apply is not required in this case to update the UI.