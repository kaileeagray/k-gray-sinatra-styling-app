## Outfit Voting Sinatra Web App
Create - Reveal - Update - Delete

look up nested relations - sketch genres, songs, artists,

# Phase 0: Build tests
  1. db tests
  2. CRUD tests - user info
  3. login authentication tests
  4. CRUD tests - outfit option
  5. voting tests

# Phase 1: Database, Model Setup
  1. sketch db tables
    users table
      + username (string)
      + email (string)
      + password digest (string)
        - more user data soon?

    event table
      + user_id (integer)
      + title (string)
      + date (date input?)
      + weather info (text)
      + description (text)

    outfit table
      + photo (use text for now? - photo - more research needed)
      + event outfit id (integer)
      + description (text)
      + votes (integer)

  2. sketch db relations
    + user has many outfits through events
    + user has many events
    + outfit belongs to event
    + event belongs to user
    - is this enough relations? do we need outfit belongs to user?

  3. build db
  4. build seeds
  5. build models
  6. text models with tux

# Phase 2: CRUD - users
  1. create new user
