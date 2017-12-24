### Hotel Reservation App built in Spring Boot and Angular 2

#### Backend endpoints test with POSTMAN:

-	__GET__
	-	http://localhost:8080/room/reservation/v1?checkin=2017-12-24&checkount=2017-12-27
	-	Result: __200 OK__ with {"id": null, "roomNumber": null, "price": null, "links": null}

-	__POST__
	-	http://localhost:8080/room/reservation/v1
	-	Body: {"id":123, "checkin":"2017-12-24", "checkout":"2017-12-27"}
	-	Result: __201 Created__ with {"id": null, "roomNumber": null, "price": null, "links": null}

-	__PUT__
	-	http://localhost:8080/room/reservation/v1
	-	{"id":123, "checkin":"2017-12-24", "checkout":"2017-12-27"}
	-	Result: __200 OK__ with {"id": null, "roomNumber": null, "price": null, "links": null}

-	__DELETE__
	-	http://localhost:8080/room/reservation/v1/123
	-	Result: __204 No Content__ with empty body

### Frontend notes:
-	By default, __ng new__ will init the project as a Git repo. Then the flag __skip-git__ should be passed.
	-	__ng new angular2 --skip-git__
		