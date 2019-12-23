# ELK_course

Software :  Elesticsearch https://www.elastic.co/

document :  https://github.com/up1/course_elk/blob/master/slide/SCK-ELK-01.pdf


## คำสั่ง CRUD 

POST , GET, PUT, DELETE 

## ตัวอย่างการใช้งาน
GET /

GET /_cat

GET /_cat/nodes?v

GET _cat/indices?v

GET /_cluster/health

PUT /store/book/1

GET /store/book/1

POST /data

DELETE /data/1


PUT student/_doc/1
{
  "id":4212010,
  "name" : "somkiat puisung",
  "major":"computer science",
  "started_dat":"2019/12/23"
  
}

GET student/_doc/1


POST student/_doc/
{
  "id":4151322,
  "name":"maae Yeng",
  "major":"Computer Business",
  "started_data": "2019/12/24"
}

GET student/_count


GET student/_search


POST student/_update/1
{
  "doc":{
    "GPA":3.01
  }
}


DELETE student/_doc/1

GET student/_doc/1

DELETE student

DELETE * //delete all index

GET student/_mapping // Show structure index 


POST _analyze
{
 "analyzer": "whitespace",
 "text": "The quick brown fox."
}

POST _analyze 
{
  "analyzer": "whitespace",
  "text": "ประเทศ ไทย"
}
