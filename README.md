# tela-de-login-coloniasemmarte
Atividade Lucas Braga
import { StyleSheet, Text, View, Pressable, Image, TextInput } from 'react-native';

export default function App() {
  return (
    <View style={styles.container}>

      <Image
        style={styles.logo}
        source={{
          uri: 'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTTg0-HeIkWJb7YggUfC9QpR_vpP4KJhpaaDJH4tr40Wg&s=10'
        }}
      />

      <Text style={styles.titulo}>🚀 COLÔNIA MARTE</Text>
      <Text style={styles.subtitulo}>Cadastro de novo colonizador</Text>

      <View style={styles.campo}>
        <Text style={styles.label}>👨‍🚀 Nome do colonizador</Text>
        <TextInput
          placeholder="Digite seu nome"
          placeholderTextColor="#9b8175"
          style={styles.input}
        />
      </View>

      <View style={styles.campo}>
        <Text style={styles.label}>🎂 Idade</Text>
        <TextInput
          keyboardType="numeric"
          placeholder="Digite sua idade"
          placeholderTextColor="#9b8175"
          style={styles.input}
        />
      </View>

      <View style={styles.campo}>
        <Text style={styles.label}>📡 E-mail</Text>
        <TextInput
          keyboardType="email-address"
          placeholder="Digite seu e-mail"
          placeholderTextColor="#9b8175"
          style={styles.input}
        />
      </View>

      <View style={styles.campo}>
        <Text style={styles.label}>🔐 Código de acesso</Text>
        <TextInput
          secureTextEntry={true}
          placeholder="••••••••"
          placeholderTextColor="#9b8175"
          style={styles.input}
        />
      </View>

      <View style={styles.campo}>
        <Text style={styles.label}>🔒 Confirmar código</Text>
        <TextInput
          secureTextEntry={true}
          placeholder="••••••••"
          placeholderTextColor="#9b8175"
          style={styles.input}
        />
      </View>

      <Pressable style={styles.botao_cadastro}>
        <Text style={styles.texto_botao}>🚀 ENTRAR NA COLÔNIA</Text>
      </Pressable>

      <Text style={styles.status}>● SISTEMA DA COLÔNIA ONLINE</Text>

    </View>
  );
}

const styles = StyleSheet.create({
  container: {
    flex: 1,
    justifyContent: 'center',
    alignItems: 'center',
    backgroundColor: '#1a0d0a',
    padding: 20,
  },

  logo: {
    width: 90,
    height: 90,
    borderRadius: 45,
    borderWidth: 3,
    borderColor: '#e85d04',
    marginBottom: 15,
  },

  titulo: {
    fontSize: 28,
    fontWeight: 'bold',
    color: '#ff6b35',
    marginBottom: 5,
    textShadowColor: '#7f2704',
    textShadowOffset: { width: 2, height: 2 },
    textShadowRadius: 5,
  },

  subtitulo: {
    fontSize: 14,
    color: '#d9a066',
    marginBottom: 30,
  },

  campo: {
    marginBottom: 12,
  },

  label: {
    color: '#f4d6bd',
    fontSize: 14,
    marginBottom: 5,
    fontWeight: 'bold',
  },

  input: {
    borderWidth: 1,
    borderColor: '#a83f12',
    borderRadius: 8,
    color: '#ffffff',
    backgroundColor: '#2b1510',
    padding: 10,
    width: 300,
  },

  botao_cadastro: {
    width: 220,
    borderRadius: 8,
    alignItems: 'center',
    padding: 13,
    marginTop: 10,
    backgroundColor: '#d94801',
    borderWidth: 2,
    borderColor: '#ff8c42',
  },

  texto_botao: {
    color: '#ffffff',
    fontWeight: 'bold',
    fontSize: 14,
  },

  status: {
    marginTop: 20,
    color: '#58d68d',
    fontSize: 11,
    fontWeight: 'bold',
  },
});
