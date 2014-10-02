talkmobile
==========

docker run -d -p 27017:27017 -p 28017:28017 --name mongodb dockerfile/mongodb mongod --noprealloc --smallfiles --rest --httpinterface
docker run -d  -p 3000:3000 --link mongodb:mongodb metakungfu/locomotive_cms:2.4.1