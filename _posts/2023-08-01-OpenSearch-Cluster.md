---
layout: post
title: OpenSearch 4개 Node로 클러스터 환경 구성해보기
date: 2023-08-01 11:00 +0800
last_modified_at: 
tags: [OpenSearch, Docker, docker-compose, Distributed System, ElasticSearch, ELK, EFK]
toc:  true
---
# Opensearch


#### Docker compose
- 원래는 기존의 싱글노드 파이프라인은 보통 AWS EC2 에서 진행하지만
- AWS EC2 Instance 의 개수를 몇 개 만들어 사용하였더니...
    - ![AWS BILLING 텍스트](/assets/img/aws_billing.png)
    - 요금이 꽤나 청구되었다. ㅜㅜ..
- 4개의 node 가 필요한 이번 pratice 는 docker-compose로 해보았다.

#### Get Start!
- [Git Hub 링크][1]
    - 해당 링크에서는 OpenSearch를 활용하여 간단한 클러스터 환경을 빠르게 구성해볼 수 있도록 해보았다.

[1]:https://github.com/Themath93/opensearch-cluster