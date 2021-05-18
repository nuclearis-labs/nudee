# Ideas iniciales

- Participantes de la plataforma reciben pagos por trabajos hechos en un ERC20 token de la plataforma
- Control de acceso a la plataforma (lista de acceso permitido y bloqueados)
- División de proyectos en subconjuntos
- Aprobación de subconjuntos por entes reguladores como ARN
- Documentos deben ser guardados con su hash.

# Dudas

- Documentación relacionados a subconjuntos puede ser almacenada descentralizada? Se debe encriptar?
- Que información es necesaria guardar en la blockchain? Alcanza un merkle tree para garantizar la autenticidad de la información?
- El ERC20 token de la plataforma debe ser el mismo para todos los proyectos, o puede ser un token NFT, para cada proyecto en curso? representando una acción.
- También se podria permitir al "cliente" de poner dinero en un contrato inteligente en forma de ETH u otra criptomoneda y que esa plata se vaya pagando a ingenieros remotos de acuerdo a los trabajos entregados. (parecido a GitCoin)

# Brainstorming

- Cada proyecto puede consistir en un merkletree de hashes de sus documentos. Abajo todos los hashes de todos los documentos. Cada vez que se suba un nuevo documento de la forma correcta se actualiza el merkle hash y cuando uno trata de alterar un documento por fuera de ese proceso y quiere luego validar lo se chequea si el merkle hash daria ok.

# Tech Stack Ideas

- GraphQL API para obtener y mutar entradas en la blockchain y BD.
- React Frontend para crear proyectos, subconjuntos y manejar documentos.
