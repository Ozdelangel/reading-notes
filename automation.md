


Roger has two txt files and they both have emails and phone numbers

We are going to reverse engineer the document(s) that were given

We are going to work with faker to generate fake data

We need to add faker to our project poetry install faker then of course we have to import faker

From faker import faker 




Fake = Faker(‘en_Us’)




Then roger is going to just look at it and it in fact an object and you can also run a print(dir(fake))

It’s going to show you all the different methods that come with it and we are going to be shown how to use all these methods




First thing if we wanted to generate some words




Fake_word = fake.word()

print(fake_word)




And you can loop through it 

For _ in range(100):

    Fake_word = fake.word()

    Print (fake_word)

You need to do this to get a whole bunch of different words




To generate a list you need to use fake.words(100) to specify how many just pass it through the functions




You can also use the same thing with sentences and paragraphs 

Fake_paragraph = fake.paragraphs(100)

print(fake_paragraph)




You can also do the same thing with anything they have in the library




We are going to create a variable thats going to hold some kind of stuff

Content = ‘’

Content += fake.paragraph()

Content += fake.email()

Content += fake.paragraph()




So roger is showing us how automation is going to take care of what is above instead of doing it manually as shown above




The way we would start is probably use a for loop




For _ in range(100):

    Content += fake.paragraph()

    Content += fake.email()

    Content += fake.paragraph()




print(content)




So we have to somehow get all this into a document

So this is going to open a text file with writing privileges




With open(‘content.txt’, ‘w+’) as f:

     f.write(content)

So what if we wanted it into an asset folder and with that we are going to use something called

shutil.copy(‘context.txt’, ‘/assets’)




How we are going to extract 

We are going to use regex