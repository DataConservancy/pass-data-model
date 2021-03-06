# Contributor

A Contributor is a person who contributed to a [Publication](Publication.md). The contributor model captures the person information as well as the roles they played in creating the publication (e.g. author).

| Field  		| Type  		| Description |
| ------------- | ------------- | ------------- |
| __id*__ | URI | Unique Person URI (autogenerated) |
| firstName | String | First name(s) of person |
| middleName | String | Middle name(s) of person |
| lastName | String | Last name(s) of person |
| displayName | String | Name for display. Separate names may not be available, but a person should always at least have a display name. |
| email | String | Contact email for person |
| orcidId | String | ORCID ID for the person |
| affiliation | String | Affiliation string for the person. Where Person is embedded in a Submission or Grant, this is the affiliation relevant to that item.  |
| roles | List[Enum] ([_see list below_](#roles-options)) | One or more roles that this Contributor performed for the associated [Publication](Publication.md) |
| publication* | URI | URI of the [Publication](Publication.md) that this person is a contributor to |
| user | URI | URI of the [User](User.md) that this Contributor represents |
 
*required 

*Properties automatically generated by the system are documented in [System Properties](SystemProperties.md). These are not available to client tools by default.*

## Roles options

These are the possible statuses for a Deposit in the order they could occur. Note that not all repositories will go through every status.

| Value  		  | Description |
| --------------- | ------------- |
| author | An author of the [Publication](Publication.md) |
| first-author | First author of the [Publication](Publication.md) |
| last-author | Last author of a [Publication](Publication.md) |
| corresponding-author | Corresponding author of a [Publication](Publication.md) |