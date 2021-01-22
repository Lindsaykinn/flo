# Models:
  # `User`
    * `has_many :songs`
    * `has_many :playlists`
    * `first_name`
    * `last_name`
    * `username`
    * `password`

  # `Song`
    * `belongs_to :artist`
    * `belongs_to :album`
    * `belongs_to :genre`
    * `title`
    * `lyrics`

  # `Playlist`
    * `has_many :songs`
    * `has_many :albums`
    * `belongs_to :user`
    * `name`

  # `Genre`
    * `has_many :songs`
    * `name`

  # `Artist`
    * `has_many :songs`
    * `belongs_to :album`
    * `name`

  # `Album`
    * `belongs_to :artist`
    * `has_many :songs`
    * `title`
    * `release_date:date`

