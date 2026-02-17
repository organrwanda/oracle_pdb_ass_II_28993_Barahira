# Oracle Pluggable Database Assignment


**Repository Link:** https://github.com/organrwanda/oracle_pdb_ass_II_28993_Barahira
**PDB Name Created:** or_PDB_28993  
**Issues Encountered:** Yes  

---

**Overview of Tasks**

This assignment involved working with Oracle Pluggable Databases (PDBs) in a Docker environment. The main objectives were:

1. **Task 1:** Create a new PDB and a user inside it.  
2. **Task 2:** Create a temporary PDB, verify it exists, and delete it completely.  
3. **Task 3:** Attempted to perform PDB operations using Linux terminal.

---

**Oracle Environment Used**

- **Oracle Version:** Oracle 21c XE (via Docker)  
- **Database Container:** gvenzl/oracle-xe  
- **Operating System:** Ubuntu (host machine)  
- **Tools:** SQL*Plus, SQL Developer  

---

**Explanation of Each Task**

**Task 1 – Create a New PDB**

- Created PDB .  
- Created a user  inside the PDB.  
- Verified that the PDB is open and the user exists.  
- Screenshot evidence included for creation, open state, and user verification.  

**Task 2 – Create and Delete a PDB**

- Created a temporary PDB 
- Verified that it exists using
- Verified deletion to confirm no residual data remains.  
- Screenshots included for creation, deletion, and verification.  

**Task 3 – Attempted Using Linux Terminal**

- Tried to perform PDB creation and deletion directly on Oracle Linux terminal.  
- Encountered multiple environment and permission issues.  
- The required Oracle XE Docker setup was necessary for proper execution.  
- This demonstrates that direct Linux terminal operations without the containerized Oracle environment are not feasible for these tasks.  

---

**Challenges Faced and Solutions**

- **Incorrect file paths:** Initially used `/u01/app/oracle/...` instead of `/opt/oracle/oradata/XE/` for Docker setup.  
  *Solution:* Adjusted paths according to Docker datafile locations.  

- **PDB staying MOUNTED:** Some PDBs did not automatically open.  
  *Solution:* Used `ALTER PLUGGABLE DATABASE <PDB_NAME> OPEN;` to bring them to `READ WRITE` mode.  


---

**Integrity Statement**

I hereby confirm that the work submitted in this assignment is entirely my own. All tasks were performed according to the instructions, and any challenges encountered were solved independently or noted appropriately.  

Signed: **Barahira Shima Organ**  
Date: **16-Feb-2026**
# oracle_pdb_ass_II_28993_Barahira
