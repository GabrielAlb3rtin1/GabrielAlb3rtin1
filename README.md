
const nome_cartao = "LU";
const numero_cartao = 12345678;
const codigo_verificador = 321;

function verificar_dados_cartao (nome, numero, codigo){
  const nome_correto = nome === nome_cartao;
  if(nome_correto){
    console.log("nome está correto");
  } else{
    console.log("nome está errado");
  }
  
  const numero_correto = numero === numero_cartao;
  if(numero_correto){
    console.log("numero está correto");
  } else{
    console.log("numero está errado");
  }
  
  const codigo_correto = codigo === codigo_verificador;
  if(codigo_correto){
    console.log("codigo está correto");
  } else{
    console.log("codigo está errado");
  }
  
  const todos_os_dados_corretos = nome_correto
      && numero_correto
      && codigo_correto;
  
  return todos_os_dados_corretos;
}
  
  const cartao_valido = verificar_dados_cartao("LU", 12345678, 123);
  console.log(cartao_valido);
  
