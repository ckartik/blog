# Systems Security for Medical Systems

###### The information here is a collection of my personal notes and notes taken for 6.858 Computer Systems Security at MIT.

Too often, the general public takes information security lightly, this is in part due to the in-effective systems in place. This creates the trade-off between having ease of access vs security in regards to personal information. This may be ok non-confidential data, however for more sensitive data it's always worthwhile to use two-factor authentication.

This set of notes will mostly pertain to the more sensitive medical data and ways to keep that data secure.

_**From a 3000 ft view of these notes, we will deal with 3 main ideas when designing secure medical information systems:**_

1. **Policy** - Deals with the set of guidelines you would like your system to follow. In computer security we follow the CIA Triad \(Here is a link to a great article [http://whatis.techtarget.com/definition/Confidentiality-integrity-and-availability-CIA\](http://whatis.techtarget.com/definition/Confidentiality-integrity-and-availability-CIA%29%29.  
   1. It is common to want to keep user information anonymised to some users on a platform. In, a more abstract sense you will want your system to limit access to information to only the intended entities. %28**Confidentiality**\)

   1. It is also common to want only certain users to have the ability to remove, add, update patient information on a system \(**Integrity**\).

   2. Possibly the most important part of a medical information system, you will want to keep the information available at all times, this can be as simple as storing medical information in a decentralised manner, many big data architectures have this feature built into it. For example, Hadoop uses a slave node architecture as part of its HDFS which allows duplicated information to be stored on multiple racks. \(**Availability**\)



