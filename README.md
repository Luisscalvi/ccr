# programa.py
qtd_aluno = int(input('Digite a quantidade de alunos da turma: '))
for aluno in range(1, qtd_aluno + 1):
    media = 0
    for avaliacao in range(1, 4):
        nota = float(input(f'Digite a nota da avaliação {avaliacao} do aluno {aluno}: '))
        media += nota
    media /= 3
    print(f'A média do aluno {aluno} foi {media:.1f}, portanto ele foi {"APROVADO" if media >= 6 else "REPROVADO"}.')
