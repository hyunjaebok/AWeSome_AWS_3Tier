## 내부 인프라

### EFS 구축
![image](https://user-images.githubusercontent.com/110655823/215499638-61a3a45f-7d66-48ac-982b-399444bbe0e7.png)
> - Autooscale된 모든 EC2(WEB/WAS)의 수정 사항 적용
> - WEB/WAS Resource를 서로 다른 EFS에 저장하여 보안 강화

</br>

### WEB/WAS 분리
![image](https://user-images.githubusercontent.com/110655823/215500133-c43b843e-8570-4c4a-af23-fb9b0dca8fe8.png)
> - 기능을 분리하여 서버 부하 방지
> - 물리적으로 분리하여 보안 강화

</br>

### Error Page 처리
![image](https://user-images.githubusercontent.com/110655823/215500665-e1515b53-73b2-4f65-8746-bb319c6513fd.png)
> - Tomcat 서비스 불능 상황의 대비

</br>

---

### [👈 Go back](https://github.com/hyunjaebok/AWeSome_AWS_3Tier_SemiProject)
