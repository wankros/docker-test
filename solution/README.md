   48  cd solution
   49  cd
   50  cd solution
   51  cd ~
   52  ls
   53  ls -l
   54  cd docker-test/
   55  ls
   56  cd solution/
   57  ls
   58  pwd
   59  ls
   60  vi gencsv.sh 
   61  chmod 755 gencsv.sh 
   62  ./gencsv.sh 
   63  ls
   64  pwd
   65  ls -lrt
   66  cat inputFile 
   67  docker run -d infracloudio/csvserver:latest
   68  docker logs e9c98f34d2416725abe9ca34b16b3e7e58387b1bb4cbfd5614382730d9830dd5
   69  pwd
   70  docker run  -itd  -v  /root/docker-test/solution/inputFile:/csvserver/inputdata  infracloudio/csvserver
   71  docker logs 83c5cd8e568eafd87da003cae58ebe4fe3033715ff17bae307be42a1396488ae
   72  docker ps
   73  docker exec -it 83c5cd8e568e bash
   74  docker ps
   75  docker stop 83c5cd8e568e
   76  docker ps
   77  docker rm 83c5cd8e568e
   78  docker logs 83c5cd8e568e
   79  docker run  -itd  -p 9393:9300 -e CSVSERVER_BORDER=Orange -v  /root/docker-test/solution/inputFile:/csvserver/inputdata  infracloudio/csvserver
   80  pwd
   81  touch README.md
   82  history > README.md 
