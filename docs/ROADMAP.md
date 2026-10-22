# Next work

## Preferred writing workflow

The user prefers direct Google Docs round trips so contributors can use document editing, grammar and spelling tools. Proposed workflow:

1. Link a lesson to a Google Doc containing research questions, answers, sources, interview questions and draft text.
2. Open in Google Docs to edit.
3. Reload from Google Docs into the builder.
4. Save builder changes to Google Docs.
5. Show last sync time, compare concurrent edits and require a merge decision rather than silently overwriting.

Implement stable lesson, question and section identifiers before sync. Question positions are not stable identifiers. Google authentication, document access, a hosted backend and conflict handling remain to be designed and implemented. Do not imply these features work yet.

## Shared persistence and recovery

- Shared database and contributor identities.
- Visible save state, edit attribution and revision history.
- Automatic backups and tested restoration.
- Preserve JSON export/import as a recovery and migration path.
- Migrate existing local answers only with clear user control.

## Photos and media

- Drag and drop photos per lesson.
- Durable object storage with captions, photographer credit, permissions and location or station metadata.
- Investigate the actual media system at baristahustle.com before selecting an integration.
- Consider media URL references first, then authenticated library search or uploads.
- Keep contributor uploads reviewable before publishing into the main media library.

## Course production decisions

- Sucafina can nominate experts across all coffee production topics.
- BH supplies useful research and interview questions, rather than asking Sucafina to plan the interviews.
- Keep filming lean: eight proposed sessions, reusing extracts across lessons; the BH roasting session is separate from origin filming.
- No recap videos or individual chapter introduction videos.
- Use the developing Terroir Map throughout regional lessons: https://brygmanden.github.io/terroirmap/
- Avoid treating point weather or elevation readings as regional ranges.
- Keep video text blue and application text orange in course document exports.

## Engineering follow ups

- Validate imported records completely and test export/import round trips.
- Move answer keys from array positions to persistent question IDs.
- Add meaningful tests for persistence, conflict detection and backups as those capabilities are built.
- Decide hosting and collaborator access before inviting Sucafina to enter substantial research.
