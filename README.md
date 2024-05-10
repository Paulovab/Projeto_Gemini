# Projeto_Gemini - Direcionamento e classificação de mensagens

Objetivo deste Projeto é receber mensagens do WhatsApp ou qualquer outro aplicativo de mensagens e direciona-las para o setor responsável por atender à aquela demanda. 

Além de direcionar para o setor responsável, o sistema vai classificar as mensagens com Prioridade Alta, Média ou Baixa.
Existe regras definidas na requisição para o GEMINI determinar as prioridades.

Este sistema vai ler as mensagens de um arquivo no formato JSON e gerar uma requisição para o GEMINI. 
Resposta do GEMINI será apresentada de forma organizada na tela, usando to_markdown().

O arquivo JSON de modelo, esta disponibilizado no Projeto.

Apresentação do Resultado:

    Comercial

        Prioridade Alta
            Gostaria de fazer uma compra de um vidro laminado.
            Vcs tem o vidro refletivo de 8mm?
            Gostaria de saber o preço de um vidro refletivo verde 10mm?
            Quero comprar um vidro incolor 8mm de 1000x1000.
        Prioridade Média
            Bom dia, quero ser atendido por um vendedor.
            Bom dia, gostaria de falar com o João.
        Prioridade Baixa
            Bom dia.
            Boa tarde, estou desde ontem aguardando um retorno da minha mensagem.

    Financeiro

        Prioridade Alta
            Bom dia, tenho um titulo em atraso e gostaria de negocia-lo.
            Boa tarde qual pix posso fazer o pagamento de um titulo?
            Boa tarde, meu titulo foi protestado, preciso falar no financeiro urgente.
        Prioridade Média
            Nenhuma mensagem.
        Prioridade Baixa
            Nenhuma mensagem.

    Marketing

        Prioridade Alta
            Bom dia, sou representante de uma empresa de publicidade e gostaria de falar com o responsável pelo marketing.
        Prioridade Média
            Nenhuma mensagem.
        Prioridade Baixa
            Nenhuma mensagem.

    RH

        Prioridade Alta
            Quero fazer parte do quadro de funcionários da empresa, para de um contato da setor responsável.
        Prioridade Média
            Nenhuma mensagem.
        Prioridade Baixa
            Nenhuma mensagem.

    Outros

        Prioridade Alta
            Bom dia, meu pedido 665555 deveria ter ficado pronto na data de ontem. Preciso deste pedido com urgência.
        Prioridade Média
            Nenhuma mensagem.
        Prioridade Baixa
            Nenhuma mensagem.

