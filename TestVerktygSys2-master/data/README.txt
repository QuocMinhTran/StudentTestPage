{
    "subjects": [], // lista med strängar på kursnamn
    "studentClasses": [], // lista med strängar på klassnamn
    "users": [
        { // user:
            "username": "",
            "password": "",
            "firstName": "",
            "lastName": "",
            "type": "", // admin, student eller teacher
            "studentClass": "", // ta bort denna om de inte används
            "subjects": [] // lista med strängar definierade i subjects
        }
    ],
    "exams": [
        { // exam
            "name": "", // namn på prov, definieras med fritext av author
            "subject": "", // alternativ på värde definieras tillgängliga värden i subjects
            "authorName": "",
            "studentName": "",
            "status": "", // done, ready eller begun
            "sentToAdmin": false,
            "startDate": "", // tilldelas nytt startdatum när student påbörjat prov
            "endDate": "", // tilldelas nytt slutdatum när student påbörjat prov
            "timeLimit": 0,
            "grade": "", // U, G eller VG
            "gScore": 0,
            "vgScore": 0,
            "questions": [
                {
                    "text": "", // frågetext
                    "type": "", // checkbox, radio, ranked
                    "answers": [
                        {
                            "text": "", // svarstext
                            "point": 1, // -1 om fel svar, annars positivt (värderat av author)
                            "checked": false, // endast relevant om type = radio eller checkbox
                            "rank": 1 // endast relevant om type = "ranked"
                        },
                        {
                            "text": "", // svarstext
                            "point": -1, // -1 om fel svar, annars positivt (värderat av author)
                            "checked": false, // endast relevant om type = radio eller checkbox
                            "rank": 0 // endast relevant om type = "ranked"
                        }
                    ]
                },
                {
                    "text": "", // frågetext
                    "type": "", // checkbox, radio, ranked
                    "answers": [
                        {
                            "text": "", // svarstext
                            "point": 0, // -1 om fel svar, annars positivt (värderat av author)
                            "checked": false, // endast relevant om type = radio eller checkbox
                            "rank": 0 // endast relevant om type = "ranked"
                        },
                        {
                            "text": "", // svarstext
                            "point": 0, // -1 om fel svar, annars positivt (värderat av author)
                            "checked": false, // endast relevant om type = radio eller checkbox
                            "rank": 1 // endast relevant om type = "ranked"
                        }
                    ]
                }
            ]
        }
    ]
}