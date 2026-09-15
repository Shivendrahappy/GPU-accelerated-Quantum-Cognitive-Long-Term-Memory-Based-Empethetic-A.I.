# GPU-accelerated-Quantum-Cognitive-Long-Term-Memory-Based-Empethetic-A.I.
Project thesis -Questions and solutions in relation to GPU accelerated Long term Memory A.I. chatbot ,whether Quantum cognitive model possible in practical model at this time ,all learning outcome and working on related model .

STEP1 - 1 Long Term memory
For long term memory we start with making dictionary 'create" as step 1 as memory 1


create = {
    'content': 'I prefer learning Python with small examples',
    'timestamp': '10 Sep 2026',
    'topic': 'learning',
    'importance': 0.8,
    'context': 'python study'
}

print(create)
     
{'content': 'I prefer learning Python with small examples', 'timestamp': '10 Sep 2026', 'topic': 'learning', 'importance': 0.8, 'context': 'python study'}

STEP 2. For set of memories - here 2nd memory is added into a list as Memory 2


create = {
    'content': 'I prefer learning Python with small examples',
    'timestamp': '10 Sep 2026',
    'topic': 'learning',
    'importance': 0.8,
    'context': 'python study'
}
memories = [create]
print (memories)
     
[{'content': 'I prefer learning Python with small examples', 'timestamp': '10 Sep 2026', 'topic': 'learning', 'importance': 0.8, 'context': 'python study'}]
STEP 3. Create is the 1st memory we have already . Now create a second memomy - memory2 About my TOEFL preparation
WE ARE CREATING SECOND MEMORY 

memory2 = {
    'content': 'I prefer learning TOEFL with small sessions of grammar ,vocab ,exersises and voice shadowing',
    'timestamp': '13 Sep 2026',
    'topic': 'learning',
    'importance': 0.9,
    'context': 'TOEFL study'
}
print(memory2)
     
{'content': 'I prefer learning TOEFL with small sessions of grammar ,vocab ,exersises and voice shadowing', 'timestamp': '13 Sep 2026', 'topic': 'learning', 'importance': 0.9, 'context': 'TOEFL study'}
STEP 4 . Put the both in a memory collection - memories= { create,memory2 )
We have tp write the full  codes for create and the memory2

create = {
    'content': 'I prefer learning Python with small examples',
    'timestamp': '10 Sep 2026',
    'topic': 'learning',
    'importance': 0.8,
    'context': 'python study'
}
memory2 = {
    'content': 'I prefer learning TOEFL with small sessions of grammar ,vocab ,exersises and voice shadowing',
    'timestamp': '13 Sep 2026',
    'topic': 'learning',
    'importance': 0.9,
    'context': 'TOEFL study'
}
memories =[create,memory2]
print(memories)
     
[{'content': 'I prefer learning Python with small examples', 'timestamp': '10 Sep 2026', 'topic': 'learning', 'importance': 0.8, 'context': 'python study'}, {'content': 'I prefer learning TOEFL with small sessions of grammar ,vocab ,exersises and voice shadowing', 'timestamp': '13 Sep 2026', 'topic': 'learning', 'importance': 0.9, 'context': 'TOEFL study'}]
