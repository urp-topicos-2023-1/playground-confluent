# playground-confluent

## Pre-requisites

Confluent URL: https://developer.confluent.io/get-started/nodejs/#configuration

## Step by step for this pklayground

### Paso 0: Crear tu propia rama

Crear rama con mi nombre
```
git checkout -b feature/ronald.requena
```

Agregar cambios y subir a Github
```
git add . 
git commit -m "initial project"
git push origin HEAD
```

### Paso 1: Crear un proyecto en blanco de Node.js

Inicializar proyecto
```
npm init
```

Obtener version de node
```
node -v
```

### Paso 2: Instalar dependencia de Kafka para Node
```
npm i node-rdkafka
```

### Paso 3: Crear archivo de properties con el nombre de getting-started.properties

Estructura del archivo
```
bootstrap.servers=< CLUSTER BOOSTRAP URL>
security.protocol=SASL_SSL
sasl.mechanisms=PLAIN
sasl.username=< CLUSTER API KEY > 
sasl.password=< CLUSTER API SECRET >
```


### Paso 4: Crear productor y consumidor

### Paso 5: Probar productor y consumidor

Prueba de Productor
```
node productor.js getting-started.properties
```