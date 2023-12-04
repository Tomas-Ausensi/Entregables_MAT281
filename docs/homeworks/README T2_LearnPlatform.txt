En caso de que se caiga el código: 
Puede que el repositorio ya se haya copiado, en ese caso, se debe comentar:

repo = g.get_repo(f"{username}/{repo_name}")
!git clone https://github.com/Tomas-Ausensi/Entregables_MAT281.git

y solo utilizar

os.chdir(repo_path)
repo_path

En otras palabras, de la celda que contiene la línea
repo = g.get_repo(f"{username}/{repo_name}")

Solo se debe utilizar 

repo_name = "Entregables_MAT281"
repo_path = "/content/" + repo_name
os.makedirs(repo_path, exist_ok=True)