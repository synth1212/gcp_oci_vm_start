# VM Lifecycle on GCP and OCI — Tutorial

## Video
Google Cloud Platform [GCP]: [Introduction Video To Create Virtual Machine](https://drive.google.com/file/d/1Ta3cMSXcutVz39Frd7cqVK_vkcEPIdvW/view?usp=sharing)

Orcale Cloud Infrastructure [OCL]: <paste link>

## Prereqs
- Cloud access to GCP and OCI
- No PHI/PII; smallest/free-tier shapes

---

## Google Cloud (GCP)
### Create
1. Console → Compute Engine → Create Instance
2. Region/Zone → Your Choice
3. Machine Type → Smallest Available/Free-Eligible
4. Image → Ubuntu LTS
5. Boot Disk → Default Minimal
6. Network → Default VPC; Ephemeral Public IP

![GCP create](images/gcp_create.png)

### Start/Stop
- Start: <State shows RUNNING>
![GCP running](images/gcp_running.png)

- Stop: <State shows TERMINATED>
![GCP terminated](images/gcp_stopped.png)

### Terminate & Verify Cleanup
- Terminate boot volume; verify cleanup

- Terminate: 
![GCP cleaned](images/gcp_terminated.png)
- Cleanup Check 
![GCP cleaned](images/gcp_clean.png)

---

## Oracle Cloud (OCI)
### Create
1. Compartment → Defult
2. Networking → VCN with Internet Connectivity (defaults)
3. Shape → Smallest/Free-Eligible
4. Image → Ubuntu (or Oracle Linux)
5. Public IP → Ephemeral
6. Boot volume → Default Minimal

![OCI create](images/oci_create.png)

### Start/Stop
- Start: <state shows RUNNING>
![OCI running](images/oci_running.png)
- Stop: <state shows STOPPED>
![OCI running](images/oci_stopped.png)

### Terminate
- Terminate boot volume; verify cleanup

- Terminate: 
![OCI cleaned](images/oci_terminated.png)
- Cleanup Check 
![OCI cleaned](images/oci_clean.png)

---

## Reflections
### Similarities
- <brief bullets>

### Differences
- <brief bullets>

### Preference (OCI vs GCP) and Why
- <one short paragraph>