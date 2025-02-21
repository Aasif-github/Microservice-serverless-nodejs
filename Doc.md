https://www.serverless.com/

> npm i serverless -g
> sls --version


2. https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html
   
How to install AWS CLI on Linux.
### **Installing AWS CLI on Ubuntu**  
The AWS Command Line Interface (AWS CLI) allows you to manage AWS services from the terminal. Follow these steps to install it on Ubuntu:

---

## **1️⃣ Update and Install Required Dependencies**  
Open a terminal and run:
```bash
sudo apt update && sudo apt install -y curl unzip
```

---

## **2️⃣ Download AWS CLI Installer**
Download the latest AWS CLI version:
```bash
curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
```

---

## **3️⃣ Extract the Installer**
```bash
unzip awscliv2.zip
```

---

## **4️⃣ Install AWS CLI**
```bash
sudo ./aws/install
```

---

## **5️⃣ Verify Installation**
After installation, check the version:
```bash
aws --version
```
Expected output:
```
aws-cli/2.x.x Python/x.x.x Linux/x86_64
```

---

## **6️⃣ Configure AWS CLI (Optional)**
If you have AWS credentials, you can configure the CLI:
```bash
aws configure
```
It will prompt for:
- **AWS Access Key ID**
- **AWS Secret Access Key**
- **Default region** (e.g., `us-east-1`)
- **Default output format** (`json`, `table`, `text`)

---

## **7️⃣ Uninstall AWS CLI (If Needed)**
```bash
sudo rm -rf /usr/local/aws-cli
rm awscliv2.zip
```

---

### 🚀 **Now you're ready to use AWS CLI on Ubuntu!**  
Run `aws help` to explore available commands. Let me know if you need help with AWS services! 😊


[Microservices Part 3](https://www.youtube.com/watch?v=jc0xKZH8bL8&list=PLaLqLOj2bk9Y0GmLjiXnX402SKYAGQiRr&index=3)