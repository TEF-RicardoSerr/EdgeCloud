# Edge Discovery APIs
These APIs fulfil the ['discovery' intents](https://github.com/camaraproject/EdgeCloud/blob/main/documentation/SupportingDocuments/Harmonisation%20of%20APIs/describing%20and%20harmonising%20the%20Edge%20APIs.md)

*Simple Edge Discovery* fulfils a single intent,  "4. I can discover the closest MEC platform to a specific terminal (closest in terms of shortest network path)"

*MEC Exposure and Experience Management* is a more comprehensive discovery API and fulfils the following intents:

### Developer intents
#### Provisioning intents 
1.	“I can retrieve a list of the operator’s MECs and their status, ordering the results by location and filtering by status (active/inactive/unknown)”
2.	"I can discover the capabilities/resources available at an operator’s MEC: CPU, Memory, Storage, GPU"
3.	"I can discover the geographical regions covered by the operators MECs"
4.	"I can discover the closest MEC platform to a specific terminal (closest in terms of shortest network path)"
5.	"I can ask the operator to provision my application server to the optimal MEC for a specific terminal, taking into account connectivity, resources (e.g. vCPU, Memory, network interfaces, storage, GPU) shortest network path, cost, network load, MEC platform load, application privacy considerations etc." 
  *  "I can ask the operator to provision my application server to all MECs that meet these criteria (note this is not focussing on a specific terminal)" 
  *  "I can ask the operator to provision my application server to a minimal set of MECs that meet these criteria across a given footprint (note this is not focussing on a specific terminal)" 
6.	 "I can ask the operator to inform me if the optimal MEC for my application and a specific terminal changes, taking into account mobility events, connectivity, shortest network path, cost, network load, MEC platform load etc."

16.	“I can ask the operator to provide the details of all the onboarded applications”
17.	"I can ask the operator to inform about the application instance details e.g., communication endpoints, resource consumed etc"


#### Runtime intents 
19.    "I can discover the closest MEC platform to a particular terminal (closest in terms of shortest network path)"
20.    "I can discover the optimal MEC platform for my application and a particular terminal, taking into account connectivity, shortest network path, cost, network load etc." (`A`)
21.    "I can discover the optimal application service endpoint for a specific terminal, taking into account mobility events, connectivity, shortest network path, cost, network load, MEC platform load etc."

### Operator intents
#### Provisioning intents
23. “I can publish an (ordered, filtered) list of my MECs, their coverage, capabilities and status” _(aligns with 1,2,3 in the developer intents)_ 
24. “I can map an application’s requirements to the best MEC for hosting it, based on application demands for CPU,Memory,Storage,GPU,bandwith,Network forecast, mobility” _(aligns with 4,5,8,9)_ 
#### Runtime intents 
25. “I can inform the developer of any event which changes which MEC is optimal for their application and connected terminals” _(aligns with  6)_

## Notes:

`A` this may not be the closest MEC, rather the 'best MEC for this job' which accounts for current MEC or network load, MEC copmute power and features etc.