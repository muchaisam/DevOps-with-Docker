

docker run -d -it --name web ubuntu sh -c 'echo "Input website:"; read website; echo "Searching.."; sleep 1; curl http://$website;'
docker exec -it web bash
root@2bb4a4404374:/# apt-get update
root@2bb4a4404374:/# apt-get install curl
root@2bb4a4404374:/# exit
docker attach web