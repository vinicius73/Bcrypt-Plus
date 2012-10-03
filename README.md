Bcrypt-Plus
===========

Classe para trabalhos com senhas em crypt () do php. Modificada apartir da classe do @TiuTalk Thiago Belem https://gist.github.com/3438461
Tudo que eu fiz foi disponibiliza-la no github e acressentar uma função de criação de senhas automáticas e aleátorias.

// Encriptando a senha <br>
$senha = 'ola mundo'; <br>
$hash = Bcrypt::hash($senha);

// Verificando a senha <br>
$senha = 'ola mundo';
$hash = '$2a$08$MTgxNjQxOTEzMTUwMzY2OOc15r9yENLiaQqel/8A82XLdj.OwIHQm'; // Valor retirado do banco  <br>
 <br>
if (Bcrypt::check($senha, $hash)) {  <br>
  echo 'Senha OK!'; <br>
} else {  <br>
	echo 'Senha incorreta!';  <br>
}  <br>
