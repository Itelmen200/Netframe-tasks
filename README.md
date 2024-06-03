## 1. Linux
# Tasks: 
1.) Get web context and monitor the system:
   To get context from a URL, you can use the wget command to download data from the URL, for example:
   ```sh
   wget https://www.google.com/
   ```
   You can also extract data using curl:
   ```sh
   curl -s https://www.google.com/ | grep "<title>"
   ```
