# CANTOR

Browser-based app for spoken audio production.

## FRAMEWORK COMPONENTS

1. AudioRecorder 
2. AudioEditor
3. Audio Annotator
4. AutoQC/AutoMaster
5. Database. (Rails / Mongo)

#### STEPS OF PRODUCTION:

##### 1. Setup the session.

* Input all reference URL(s)
* Title
* Narrator
* Author (if different from c.)

##### 2. Recording.

* Record 10sec of silence
* Display reference URLs in left pane. Prompt reader to make edits to reference URL.
* Record all narration material. Save only those recordings that user explcitly indicates.

##### 3. Proofing.

* From each file, select regions you want to keep for your final production.
* Also select regions you want to re-record. Add a note and hit save.

##### 4. Editing.

* After verifying all pickups have been fixed with a re-record, we may move on to this step.
* Each audio file is presented to the user for editing/cleanup. 
* Compile all clips into a single audio file.
* Take the full-length production and allow user to insert/remove room tone where needed to change pacing.

##### 5. AutoMaster.

* 1 sec at top and tail of file
* Meets dynamics specs
* Output a WAV, an OGG, and an OPUS.