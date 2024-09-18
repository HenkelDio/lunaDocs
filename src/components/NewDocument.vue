<template>
    <div class="container" style="overflow: auto;">
        <!-- Header -->
        <div class="header">
          <div
          style="border: 1px solid black; height: 129px; display: flex; padding: 0 10px;
          margin-top: 10px;">
            <img src="../assets/logo.svg" alt="Logo Pró-Memória">
          </div>
            <div class="header-table">
              <table>
                    <tr>
                        <td
                          style="font-weight: bold; text-align: center;">
                          Procedimento Operacional Padrão
                        </td>
                    </tr>
                    <tr>
                        <td style="font-weight: bold;  text-align: center;">Atendimento ao Cliente
                      </td>
                    </tr>
                </table>
            </div>
            <div class="header-info">
                <table>
                    <tr>
                        <th>Código:</th>
                        <td>POP-OPR-010</td>
                    </tr>
                    <tr>
                        <th>Revisão:</th>
                        <td>01</td>
                    </tr>
                    <tr>
                        <th>Data:</th>
                        <td>01.02.2011</td>
                    </tr>
                    <tr>
                        <th>Página:</th>
                        <td>1 de 6</td>
                    </tr>
                </table>
            </div>
        </div>
        <!-- Objetivo -->
        <div class="section">
            <h3>1. OBJETIVO</h3>
            <p>Estabelecer as diretrizes básicas pertinentes ao atendimento aos clientes
              mantenedores de documentos nas instalações internas da PRÓ-MEMÓRIA.</p>
        </div>

        <!-- Aplicação -->
        <div class="section">
            <h3>2. APLICAÇÃO</h3>
            <p>Este procedimento aplica-se a toda a documentação produzida ou recebida
               pelos clientes custodiados pela PRÓ-MEMÓRIA.</p>
        </div>

        <!-- Definições -->
        <div class="section">
            <h3>3. DEFINIÇÕES</h3>
            <ul>
                <li><strong>Cliente Custodiante:</strong> cliente que possui documentos
                  custodiados pela PRÓ-MEMÓRIA, quer seja em instalações próprias, quer
                  seja nas instalações da PRÓ-MEMÓRIA.</li>
                <li><strong>Empréstimo:</strong> processo de disponibilizar documentos
                  sob sua custódia ao cliente, desde que comprovada a necessidade.</li>
                <li><strong>Registro de Empréstimo:</strong> documento que registra a
                  realização de um empréstimo de documentos.</li>
            </ul>
        </div>

        <!-- Descrição das Atividades -->
        <div class="section">
            <h3>4. DESCRIÇÃO DAS ATIVIDADES</h3>
            <h4>4.1. AUTORIZAÇÃO/CREDENCIAMENTO DE USUÁRIOS
              PARA CONSULTA E/OU EMPRÉSTIMO DE DOCUMENTOS</h4>
            <p>a) Os clientes que possuem documentos custodiados
              deverão enviar à PRÓ-MEMÓRIA uma relação de usuários autorizados
              para realizar consultas ou empréstimos de documentos.</p>
            <p>b) Cada usuário deverá ser identificado por nome completo e função.</p>
        </div>

    </div>
</template>

<style lang="scss">
        .header {
            display: flex;
            align-items: center;
            justify-content: center;
            flex-direction: row;
            border-bottom: 2px solid black;
            padding-bottom: 10px;
            margin-bottom: 20px;
        }
        .header img {
            width: 100px;
        }
        .header-table table {
            width: 400px;
            height: 129px;
            border: 1px solid black;
            border-collapse: collapse;
        }
        .header-info {
            text-align: right;
        }
        .header-info table {
            width: 100%;
            border: 1px solid black;
            border-collapse: collapse;
        }
        .header-info th, .header-info td {
            border: 1px solid black;
            padding: 5px;
            text-align: left;
        }
        h1, h2, h3 {
            text-align: center;
            font-size: 1.5rem;
        }
        .section {
            margin-bottom: 20px;
        }
        .section h3 {
            background-color: #f2f2f2;
            padding: 10px;
            border-left: 5px solid red;
        }
        table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 10px;
        }
        th, td {
            border: 1px solid black;
            padding: 8px;
            text-align: left;
        }
</style>
