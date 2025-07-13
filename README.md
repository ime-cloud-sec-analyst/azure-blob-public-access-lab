# azure-blob-public-access-lab
Azure Blob Storage Lab - Uploading, configuring public access, and accessing blobs via direct URL. Includes task1b.txt demonstrating AWS CloudFormation VPC YAML format.
# Azure Blob Storage Lab – Public Access and Blob Retrieval

## 📌 Overview

This lab demonstrates how to use **Azure Blob Storage** to:
- Create a storage account and a blob container.
- Upload a `.txt` file (task1b.txt).
- Configure access to make the blob publicly accessible via a direct URL.
- Test the public access through a web browser.

The file uploaded contains a sample AWS CloudFormation template (`task1b.txt`) for provisioning a VPC with a public subnet and Internet Gateway—highlighting hybrid knowledge across AWS and Azure.

---

## 🎯 Objective

- Understand Azure Blob Storage configuration and access levels.
- Practice uploading blobs through the Azure Portal.
- Test public access and permissions.
- Document and validate cloud file hosting processes.

---

## 🔍 Scope

This hands-on lab was executed using:
- **Azure Storage Account (StorageV2)**  
- **Azure Portal (Web UI)**  
- **Blob container (Hot Tier, Public Access)**  
- **Blob file:** task1b.txt containing an AWS CloudFormation skeleton.

---

## 🛠️ Tools and Services

- **Microsoft Azure Portal**
- **Azure Storage Account**
- **Azure Blob Storage**
- **Azure CLI (optional for future automation)**
- **GitHub (for documentation)**

---

## 🧪 Step-by-Step Process

### 1. **Create a Storage Account**
- Chose *StorageV2 (General Purpose v2)* with Hot tier.
- Allowed anonymous access.
- Used standard performance and default options.

### 2. **Create a Blob Container**
- Created `mycontainer` in the storage account.
- Uploaded `task1b.txt` to the container.

### 3. **Set Access Level**
- Configured blob to be **publicly accessible**.
- Verified the access level by copying and visiting the blob’s URL.

### 4. **Access the Blob Publicly**
- Accessed via:

- https://demostorageime123.blob.core.windows.net/mycontainer/task1b.txt

- - Confirmed the file is viewable in browser without authentication.

### 5. **GitHub Repository Setup**
- Created a public repository.
- Uploaded screenshots and `task1b.txt`.
- Documented the process with a professional README file.

---

## ⚠️ Limitations

- Cannot change access level for some containers after creation unless recreated.
- If anonymous access is disabled at the storage account level, public URLs will be blocked.
- No versioning or redundancy tested in this lab.
- Limited to Azure Portal UI – CLI/ARM/Bicep not explored in this version.

---

## ✅ Outcome / Success

- Blob container was successfully created and made public.
- File was publicly accessible via URL.
- Demonstrated cross-cloud understanding by referencing AWS VPC setup.
- Repository created to document and share lab result.

---

## 📚 Lessons Learned

- Blob storage access must be managed both at the **account level** and **container level**.
- Public access can be tricky: Azure has enhanced restrictions to avoid accidental data leaks.
- Always test the access URL from an **incognito window** to ensure it’s truly public.
- GitHub is a great platform for lab documentation and cloud portfolio.

---

## 📌 Files Included

| File            | Description                                |
|-----------------|--------------------------------------------|
| task1b.txt      | Sample AWS VPC CloudFormation YAML         |
| /screenshots    | Azure portal screenshots for all steps     |

---

## 🌐 Author

**Ime Ben**  
Cloud Security Analyst  
GitHub: [ime-cloud-sec-analyst](https://github.com/ime-cloud-sec-analyst)  
Email: imegcu55@gmail.com

---

## 📁 Repository URL

[https://github.com/ime-cloud-sec-analyst/azure-blob-public-access-lab](https://github.com/ime-cloud-sec-analyst/azure-blob-public-access-lab)

---

## 📎 References

- [Azure Blob Storage Documentation](https://learn.microsoft.com/en-us/azure/storage/blobs/)
- [GitHub README Guide](https://www.makeareadme.com/)
- [AWS CloudFormation Template Anatomy](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/template-anatomy.html)

---


