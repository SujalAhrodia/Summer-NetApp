# na_ontap_clus_peer : Cluster Peering

## Structure:
* Two single node clusters running 9.5.
* Create aggregates on both of them.
* Create data vservers on both the clusters to perform svm peering.
 
## Note:
* Tested for ONTAP v.9.5
* Configures intercluster LIFS on shared data ports
  * Other options: dedicated ports, custom IPspaces
* Differences in various versions of ONTAP
  * Before 9.3: need to know the intercluster LIFs of the remote cluster in advance.
  * After 9.3: can use 'generate passphrase' feature for peering without knowing LIFs in advance.  
  * After 9.6: Cluster peering encryption is enabled (not part of this role).
* SVM peering requires cluster peering.

