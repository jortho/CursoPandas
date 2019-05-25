# Resumen de comandos de Pandas y Python.

. un dataframe es un conjunto de series como columnas

Busquedas y selecciones:

df.head(x)

df=pd.DataFrame(columns=['Pais'])

Selección:

 df[df.nombre == 'contenido']


Df.iloc: busca por posiciones de filas y columnas

Df.loc: busca por nombres de columnas.

procesos[procesos.Area.str.contains('D')]

for columna in range(len(aplicaciones.columns)):
    for fila in range(len(chile.index)):
        print('c: ', columna, ' F: ', fila)
        dato = buscar(chile.iloc[columna,fila])
        if dato.empty == False:
            print('dato: ', dato)
            print(celda, 'valor: ', dato)
            print('chile: ', chile.iloc[columna,fila])


aplicaciones.iterrows(): itera sobre filas. Fila, serie.

df.append({'Pais': ['españa','italia']}, ignore_index=True): añade una lista de valores a un DF

zip(['one', 'two', 'three'], [1, 2, 3]))


# count the number of NaN values in each column
   df.isnull().sum()

df[df.Proceso.isnull()]

df[df.Proceso.notnull()]

if diccio.get('key', 'no esta') != 'no esta':

def addword(word, pagenumber):
    try: theIndex[word].append(pagenumber) 
    except KeyError: theIndex[word] = [pagenumber]

Es lo mismo que:

def addword(word, pagenumber):    
	theIndex.setdefault(word, []).append(pagenumber)

