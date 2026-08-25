# Store UTC, render local, and never do arithmetic on local time

Market calendars break on daylight-saving transitions when local timestamps are added or subtracted. Keeping every stored instant in UTC and converting only at the display boundary removes an entire class of off-by-one-hour bugs around DST changeovers.
