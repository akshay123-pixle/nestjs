client->>controller(request)->>service(logic that sends to controller)->>


dependency injecttion

dependency-(one class is depends on another class)

injcetion( inject that one to another since they are dependent)

these things happen automatically by nestjs


Importatnt
(Video-12)
# DTO- data transfter object
DTO in nest JS and it does not apply stricy validation by default we have to to explictly mention the DTO while run time since TS does not apply bydefalt, 

steps to follow
1)npm  i class-validator class-transformer
validator->on instance
tranformer-> on objects(JSON)

2) add IsString or IsInt or IsBoolean in DTO file

3) also make it globally available in main.ts



# Custom pipes-> transform or validate incoming data(its runs befoe exuecution of controller )
video-13

own customer pipes we can create
can be apply on globally,method levele and controller too

steps->
01
nest g pipe common/pipes/uppercase




# protecting routes
-> u protech the routes like logged-in ,useror admin can access them likewise
if user is not login then it cant access the resources


# guards->>
to protecg the routes u can use the guards,
classess to  implement if req allow orr not

they ececute before controller
step 01->>nest g guard guards/auth




# exception

nest g filter filters/http-execption


# middleware
 nest g middleware middleware/logger