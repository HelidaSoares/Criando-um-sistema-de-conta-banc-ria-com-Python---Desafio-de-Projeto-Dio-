# Criando-um-sistema-de-conta-banc-ria-com-Python---Desafio-de-Projeto-Dio-
class Cliente:
def__init__(Self,nome,cpf):
Self.nome = nome
Self.cpf = cpf

class Conta:
def__init__(self,numero,cliente,saldo=0):
Self.numero = numero
Self.cliente = saldo
Self.transacoes = []

def depositar (self,valor):
if valor >0:
  Self.saldo += saldo
  Self.transacoes.append (f"Depósito: + R${valor:.2f}")
  print (f"Depósito de R${valor:.2f} realizado com sucesso.")
  else:
  print ("valor de depósito inválido!")

  def sacar (self,valor):
  if 0< valor <= self.saldo:
  Self.saldo-= valor
  Self.transacoes.append(f"saque: -R${valor:.2f}")
  print (f"saque de R${valor:.2f} realizado com sucesso.")
  else:
  print ("valor de saque inválido ou saldo insuficiente!")

def extrato (self):
  print (f"extrato da conta{self.numero} - Cliente:{self.cliente.nome}")
  for transacao in self.transacoes:
  print (transacao)
  print (f"saldo atual: R${self.saldo:.2f}")

class Banco:
def__init__(self):
Self.contas = {}

def criar_conta (self,numero,cliente):
if numero not in self.contas:
nova_conta = Conta (numero, cliente)
self.contas [numero] = nova_conta
print (f"Conta{numero} criada com sucesso para {cliente.nome}.")
else:
print ("Numero de conta já existente!")

def buscar_contas (self,numero):
return self.contas.get (numero,Nome)

# Uso do sistema bancário 
banco = Banco()

# Criando clientes
cliente1 = Cliente ("Helida","123.456.789-00")
cliente2 = Cliente ("Tilli","987.654.321-00")

# Criando contas para os clientes 
banco.criar_conta (1001,cliente1)
banco.criar_conta (1002,cliente2)

# Realizando transações 
conta1 = banco.buscar_conta (1001)
if conta1:
   conta1.depositar (500)
   conta1.sacar (200)
   conta1.extrato ()

conta2 = banco.buscar_conta (1002)
if conta2:
   conta2.depositar (1000)
   conta2.sacar (150)
   conta2.extrato ()
   
























  



  



  




