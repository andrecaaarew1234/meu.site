import requests

# URL da imagem (substitua pela URL real ou use bytes recebidos)
image_url = "COLE_AQUI_A_URL_DA_IMAGEM"

# Salvar localmente
response = requests.get(image_url)
with open("sprite.png", "wb") as f:
    f.write(response.content)

print("Imagem salva como sprite.png")
