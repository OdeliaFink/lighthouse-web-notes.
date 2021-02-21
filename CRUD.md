# CRUD

app.get('/objectives', (req,res) => { //GET ALL THE objectives }) app.get('/objectives/new', (req,res) => { //GET A FORM TO CREATE A NEW MEME })

app.post('/objectives', (req,res) => { // TAKE THE INFORMATION FROM A FORM // AND SAVE IT ( POST saves ) })

app.get('/objectives/:id', (req,res) => { //SHOW A SPECIFIC MEME })

app.post('/objectives/:id', (req,res) => { //EDIT and SAVE the SEPCIFIC MEME })

app.post('/objectives/:id/delete', (req,res) => { //DELETE A SPECIFIC MEME })