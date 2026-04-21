실행
	open -a Docker

docker images
docker run -d -p 8888:8080 searxng/searxng
docker ps
docker exec -it <docker 이름> sh
	이후 수정이든 뭐든 하면 됨.
	vi /etc/searxng/settings.yml
		여기 formats 아래 json 추가함
	이후 컨테이너 재시작
		docker restart <docker 이름>
