`git clone ...`
`cd test_savon`
`bundle`
`bundle exec ruby ./test.rb`

Script will create copy of message "Green Template Message" with identical HTML and subject
Then it fetches HTML of newly created message and save both messages HTML content into
local directory in files: `new_copied_message.html` and `original_message.html`

`diff original_message.html new_copied_message.html` shows they are identical

Now go to UI, find message named 'New Copied Message [latest_time_stamp]' and try
edit its HTML content. You will see it is very different than original message has.
