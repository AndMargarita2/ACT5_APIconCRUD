# ACT5_APIconCRUD

@app.get("/alumnos")
parametros:
  {       
        Nombre (string),
		    Matricula (int),
		    Edad (int),
		    Facultad (string),
		    Grado (string),
		    Carrera (string),
		    Genero (string),
		    Correo (string),
		    Promedio (float),
		    Semestre (integer)
		 }
Respuesta:
,
{
  "Nombre": "Andrea Maldonado Morales",
  "Matricula": 202233003,
  "Edad": 23,
  "Facultad": "Ciencias de la computación",
  "Grado": "Licenciatura",
  "Carrera": "Ing. Tecnologias de la Informacion",
  "Genero": "Femenino",
  "Correo": "andrea.maldonado@alumno.buap.mx",
  "Promedio": 8.3,
  "Semestre": 6
}
,

@app.post("/alumnos/")
parametros:
    {       
        Nombre (string),
		    Matricula (int),
		    Edad (int),
		    Facultad (string),
		    Grado (string),
		    Carrera (string),
		    Genero (string),
		    Correo (string),
		    Promedio (float),
		    Semestre (integer)
		 }
respuesta:
{
  "Nombre": "Martita",
  "Matricula": 20204444,
  "Edad": 25,
  "Facultad": "Ciencias de la computación",
  "Grado": "Licenciatura",
  "Carrera": "Lic. Ciencias Computación",
  "Genero": "Femenino",
  "Correo": "pepe.pp@alumno.buap.mx",
  "Promedio": 10,
  "Semestre": 10
}

@app.put("/alumnos/")
parametros:
    {       
        Nombre (string),
		    Matricula (int),
		    Edad (int),
		    Facultad (string),
		    Grado (string),
		    Carrera (string),
		    Genero (string),
		    Correo (string),
		    Promedio (float),
		    Semestre (integer)
		 }
respuesta:
{
  "Nombre": "Martita",
  "Matricula": 20204444,
  "Edad": 25,
  "Facultad": "Ciencias de la computación",
  "Grado": "Licenciatura",
  "Carrera": "Lic. Ciencias Computación",
  "Genero": "Femenino",
  "Correo": "marta.mm@alumno.buap.mx",
  "Promedio": 10,
  "Semestre": 10
}

@app.delete("/alumnos/{matricula}")
parametros:
Matricula (int)

respuesta:
{
  "mensaje": "Alumno con matrícula 20204444 eliminado correctamente"
}
