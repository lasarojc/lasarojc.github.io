---
layout: post
categories:
 - Publications

title: AR2C2 - Actively Replicated Controllers for SDN resilient Control Planes
author: Eros S. Spalla, Diego Rossi Mafioletti, Alextian Bartolomeu Liberato, Gilberto Ewald, Christian Esteve Rothenberg, Lásaro Camargos, Rodolfo Villaca, Magnos Martinello
venue: NOMS 2016 - 2016 IEEE/IFIP Network Operations and Management Symposium 
paper: 10.1109/NOMS.2016.7502812
type: Peer-reviewed Conference

---
Abstract: Software Defined Networking (SDN) is a promisingarchitectural  approach  based  on  a  programmatic  separation  ofthe  control  and  data  planes.  For  high  availability  purposes,logically  centralized  SDN  controllers  follow  a  distributed  im-plementation.  While  controller  role  features  in  the  OpenFlowprotocol allow switches to communicate with multiple controllers,these mechanisms alone are not sufficient to guarantee a resilientcontrol  plane,  leaving  the  actual  implementation  an  open  chal-lenge for SDN designers. This paper explores OpenFlow roles forthe  design  of  resilient  SDN  control  plane  and  proposes  AR2C2as  an  actively  replicated  multi-controller  strategy.  As  proof  ofconcept,  AR2C2  is  implemented  based  on  the  Ryu  controllerand  relying  on  OpenReplica  to  ensure  consistent  state  amongthe   distributed   controllers.   Our   prototype   is   experimentallyevaluated  using  real  commodity  switches  and  Mininet  emulatedenvironment.  Results  of  the  measured  times  to  recover  fromfailures for different workloads shed some light on the practicaltrade-offs on replication overhead and latency as a step forwardtowards  SDN  resiliency. 

