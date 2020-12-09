# EmpresaMudanzas
el notas
Create table empleado
(
id_empleado int,
nombre varchar (10),
direccion varchar (20),
tel_contacto varchar (11),
primary key (id_empleado)
);

insert into empleado values
(1,'luis','caracas','0995830143'),
(2,'ronald','los bajos','0994828528'),
(3,'cobos','portoviejo','0994429869'),
(4,'aguirre','monstecriti','0988408329'),
(5,'guillermo','manta','0993908703');


Create table empresa

(id_empresa int,
nombre varchar (15),
direccion varchar (20),
telefono varchar (10),
primary key (id_empresa) );

insert into empresa values
(1001,'Kusko','caracas','0995830143'),
(2002,'Flu','los bajos','0994828528'),
(3003,'Kya','portoviejo','0994429869'),
(4004,'abocado','monstecriti','0988408329'),
(5005,'turki','manta','0993908703');


create table vehiculo
(
id_empleado int,
id_vehiculo int,
id_empresa int,
vehiculo varchar (15),
tipo_vehiculo varchar (15),
primary key (id_empleado));

insert into vehiculo values
(1,101,1001,'sedan','normal'),
(2,102,2002,'chevrolet','camioneta'),
(3,103,3003,'kia','sport'),
(4,104,4004,'mazda','sport'),
(5,105,5005,'rio','unitario');
Select e.nombre, e.direccion, v.vehiculo from empresa e, vehiculo v where e.id_empresa = v.id_empresa
Select e.nombre, e.direccion, v.vehiculo from empleado e, vehiculo v where e.id_empleado = v.id_empleado

select * from vehiculo
