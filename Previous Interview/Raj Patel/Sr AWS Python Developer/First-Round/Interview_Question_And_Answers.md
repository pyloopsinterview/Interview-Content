Here is the **Markdown file content** exactly as you requested.
You can copy & paste it directly into a `.md` file.

---

# **AWS Python Coding Questions & Solutions**

## **Question 1**

**Write a Python script using boto3 to check if a specific S3 bucket exists.
If the bucket exists → print “Bucket exists”.
Otherwise → print “Bucket does not exist”.
Handle errors gracefully.**

### **Solution**

```python
import boto3
from botocore.exceptions import ClientError

def check_bucket_exists(bucket_name):
    s3 = boto3.client("s3")

    try:
        s3.head_bucket(Bucket=bucket_name)
        print("Bucket exists")
    except ClientError as e:
        code = e.response["Error"]["Code"]
        if code in ["404", "NoSuchBucket"]:
            print("Bucket does not exist")
        elif code in ["403", "AccessDenied"]:
            print("Access denied to bucket")
        else:
            print(f"Unexpected AWS error: {e}")

# Example call
check_bucket_exists("my-test-bucket")
```

---

## **Question 2**

**Write a Python script using boto3 to list all objects in a specific S3 bucket and print their sizes in bytes.
Handle errors such as missing bucket or insufficient permissions.**

### **Solution**

```python
import boto3
from botocore.exceptions import ClientError

def list_objects_with_size(bucket_name):
    s3 = boto3.client("s3")

    try:
        resp = s3.list_objects_v2(Bucket=bucket_name)

        if "Contents" not in resp:
            print("Bucket is empty.")
            return

        for obj in resp["Contents"]:
            print(f"{obj['Key']} -> {obj['Size']} bytes")

    except ClientError as e:
        code = e.response["Error"]["Code"]
        if code in ["404", "NoSuchBucket"]:
            print("Bucket does not exist.")
        elif code == "AccessDenied":
            print("Access denied to bucket.")
        else:
            print(f"AWS Error: {e}")

# Example call
list_objects_with_size("my-test-bucket")
```

---

If you want this exported as a **downloadable .md file**, just say **"export this as md"** and I’ll generate the file for you.
