# Reflection

This laboratory activity helped me understand the importance of cloud storage and how it is used to manage different types of data. I learned that Object Storage is better suited for storing millions of photos because it is designed for large amounts of unstructured data. Unlike traditional Block Storage, object storage can store files as objects with their own metadata and can scale when the amount of data increases. This makes it useful for applications that allow users to upload many images.

Docker made it easier for me to deploy MinIO because I did not have to manually install and configure all the required components. By using a Docker command, I was able to download the MinIO image, create a container, and configure the ports and login credentials. This made the deployment process faster and easier to manage.

I also learned that a bucket is a container used to organize and store objects in object storage. In this activity, I created a bucket named `client-photos` and uploaded a sample file into it. This helped me understand how files are organized in an object storage system.

Large companies can prevent object-storage data loss by keeping multiple copies of data and using replication across different servers or locations. They can also use backups and redundancy so that the data can still be recovered if a physical server crashes. This shows why cloud storage is useful for protecting important data.

Lastly, my confidence with the Linux command line is improving. At first, I was not very familiar with commands and sometimes entered commands incorrectly. After using commands such as `docker`, `ls`, `cd`, and `git`, I became more comfortable working in the terminal. This activity helped me become more confident in using Linux for cloud-related tasks.
