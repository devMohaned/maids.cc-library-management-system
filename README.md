This is a task for Maids.cc for Backend Development using Java & Spring Boot.

Clone the Project using your IDE (I am using Intellj)

run the project

run the unit test for descriptive examples

<details><summary>How to interact with the API endpoints?</summary>
  #1 Copy The Collection for Postman


  #2 Save it into a file with extension ".postman_collection" i.e: api-collection.postman_collection


  #3 Drag it into Postman


  #4 Run Whatever APIs you want or customize the request

</details>

To get the collection, click below this line
============================================

<details><summary>#1 Copy The Collection for Postman</summary>
{
	"info": {
		"_postman_id": "111c5404-d324-49b2-998a-745151548d00",
		"name": "Maids.cc",
		"schema": "https://schema.getpostman.com/json/collection/v2.1.0/collection.json",
		"_exporter_id": "23277089"
	},
	"item": [
		{
			"name": "Books",
			"item": [
				{
					"name": "Get All Books",
					"request": {
						"method": "GET",
						"header": [],
						"url": {
							"raw": "localhost:8080/api/books",
							"host": [
								"localhost"
							],
							"port": "8080",
							"path": [
								"api",
								"books"
							]
						}
					},
					"response": []
				},
				{
					"name": "Get Specific Book",
					"request": {
						"method": "GET",
						"header": [],
						"url": {
							"raw": "localhost:8080/api/books/1",
							"host": [
								"localhost"
							],
							"port": "8080",
							"path": [
								"api",
								"books",
								"1"
							]
						}
					},
					"response": []
				},
				{
					"name": "Save a Book",
					"request": {
						"method": "POST",
						"header": [],
						"body": {
							"mode": "raw",
							"raw": "{\r\n    \"title\": \"Clean Code Architecture\",\r\n    \"author\": \"Robert Martin\",\r\n    \"isbn\": \"978-1-56619-909-4\",\r\n    \"publicationYear\": 2017,\r\n    \"quantity\": 5\r\n\r\n\r\n}",
							"options": {
								"raw": {
									"language": "json"
								}
							}
						},
						"url": {
							"raw": "localhost:8080/api/books",
							"host": [
								"localhost"
							],
							"port": "8080",
							"path": [
								"api",
								"books"
							]
						}
					},
					"response": []
				},
				{
					"name": "Update a Book",
					"request": {
						"method": "PUT",
						"header": [],
						"body": {
							"mode": "raw",
							"raw": "{\r\n    \"title\": \"Clean Code Agile\",\r\n    \"author\": \"Robert Martin\",\r\n    \"isbn\": \"978-1-56619-909-4\",\r\n    \"publicationYear\": 2017,\r\n    \"quantity\": 20\r\n\r\n\r\n}",
							"options": {
								"raw": {
									"language": "json"
								}
							}
						},
						"url": {
							"raw": "localhost:8080/api/books/1",
							"host": [
								"localhost"
							],
							"port": "8080",
							"path": [
								"api",
								"books",
								"1"
							]
						}
					},
					"response": []
				},
				{
					"name": "Delete a Book",
					"request": {
						"method": "DELETE",
						"header": [],
						"url": {
							"raw": "localhost:8080/api/books/1",
							"host": [
								"localhost"
							],
							"port": "8080",
							"path": [
								"api",
								"books",
								"1"
							]
						}
					},
					"response": []
				}
			]
		},
		{
			"name": "Patrons",
			"item": [
				{
					"name": "Get All Patrons",
					"request": {
						"method": "GET",
						"header": [],
						"url": {
							"raw": "localhost:8080/api/patrons",
							"host": [
								"localhost"
							],
							"port": "8080",
							"path": [
								"api",
								"patrons"
							]
						}
					},
					"response": []
				},
				{
					"name": "Get Specific Patron",
					"request": {
						"method": "GET",
						"header": [],
						"url": {
							"raw": "localhost:8080/api/patrons/1",
							"host": [
								"localhost"
							],
							"port": "8080",
							"path": [
								"api",
								"patrons",
								"1"
							]
						}
					},
					"response": []
				},
				{
					"name": "Save a Patron",
					"request": {
						"method": "POST",
						"header": [],
						"body": {
							"mode": "raw",
							"raw": "{\r\n    \"name\": \"Mohaned Ashraf\",\r\n    \"contactInfo\": \"A way of communication, number or email or whatever of your choice\"\r\n}",
							"options": {
								"raw": {
									"language": "json"
								}
							}
						},
						"url": {
							"raw": "localhost:8080/api/patrons",
							"host": [
								"localhost"
							],
							"port": "8080",
							"path": [
								"api",
								"patrons"
							]
						}
					},
					"response": []
				},
				{
					"name": "Update a Patron",
					"request": {
						"method": "PUT",
						"header": [],
						"body": {
							"mode": "raw",
							"raw": "{\r\n    \"name\": \"Mohaned Ashraf\",\r\n    \"contactInfo\": \"Updated Contact Info\"\r\n}",
							"options": {
								"raw": {
									"language": "json"
								}
							}
						},
						"url": {
							"raw": "localhost:8080/api/patrons/1",
							"host": [
								"localhost"
							],
							"port": "8080",
							"path": [
								"api",
								"patrons",
								"1"
							]
						}
					},
					"response": []
				},
				{
					"name": "Delete a Patron",
					"request": {
						"method": "DELETE",
						"header": [],
						"body": {
							"mode": "raw",
							"raw": "",
							"options": {
								"raw": {
									"language": "json"
								}
							}
						},
						"url": {
							"raw": "localhost:8080/api/patrons/1",
							"host": [
								"localhost"
							],
							"port": "8080",
							"path": [
								"api",
								"patrons",
								"1"
							]
						}
					},
					"response": []
				}
			]
		},
		{
			"name": "Borrow a Book",
			"request": {
				"method": "POST",
				"header": [],
				"url": {
					"raw": "localhost:8080/api/borrow/1/patron/1?return-date=2024-05-15",
					"host": [
						"localhost"
					],
					"port": "8080",
					"path": [
						"api",
						"borrow",
						"1",
						"patron",
						"1"
					],
					"query": [
						{
							"key": "return-date",
							"value": "2024-05-15"
						}
					]
				}
			},
			"response": []
		},
		{
			"name": "Return a Book",
			"request": {
				"method": "PUT",
				"header": [],
				"url": {
					"raw": "localhost:8080/api/return/1/patron/1",
					"host": [
						"localhost"
					],
					"port": "8080",
					"path": [
						"api",
						"return",
						"1",
						"patron",
						"1"
					]
				}
			},
			"response": []
		}
	]
}
</details>
