# Secure Semantic Search in the Cloud (S3C)

This is an open-source program that enables semantic enterprise search for unstructured datasets stored in the cloud. 
If you are using this tool in your research projects, please cite the following paper:
```
@inproceedings{woodworth2016s3c,
  title={S3C: An architecture for space-efficient semantic search over encrypted data in the cloud},
  author={Woodworth, Jason and Salehi, Mohsen Amini and Raghavan, Vijay},
  booktitle={Proceedings of the 4th IEEE International Conference on Big Data},
  series={Big Data'16},
  pages={3722--3731},
  year={2016},
  month={December}
}
```
The paper is also available in the following URL:
http://hpcclab.org/paperPdf/bigdata16/bigdata16.pdf

Below, you can find the steps to execute the program:
1. To provide full access to the project folder: chmod a+x "/path/to the downloaded/folder/and/its contens.  for example:
```chmod a+x /home/S3C/*``` 
2. Execute script "./exec.sh" to create folder + unzip demo dataset. 
3. Check 'cloud' folder is created in the parent folder. That means script runs succeffully. 
4. Open Eclipse on other Java IDE
5. Import two project:
 	a.Open Project -> Path to S3C -> Semantic Search Client
        b.a.Open Project -> Path to S3C -> Semantic Search Cloud 

6. Run cloud project -> (Main class: SemanticSearchCloud.java)
7. Run client project -> (Main class: SemanticSearchClient.java)
MY TASK: Upload modified s3c to github now.
8. 
   a. Type "-u" in client console.
   b. Provide the upload path. Type "input/demo_dataset". Our demo dataset is ready to be uploaded. 


9. After uploading, stop client execution. At this time, server has already built index and docSize. 

10. Re-run client project. Type "-s" to search over the index.

11. From the result, keep a note of the file (s) that you want to decrypt. 
12. Go to Semantic Search Client -> uploads folder. Copy those files into semantic Search Client -> data-> input_encrypted folder.
13. Re-run Client project. Choose '-d' to dectrypt resulted document. Insert file_name.txt. 
14. After getting successful message, go to semantic Search Client -> data-> output_decrypted folder. Open the decrypted file to read the content!!






