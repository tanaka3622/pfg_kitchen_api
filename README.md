# PdfKitchen

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'pdf_kitchen'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install pdf_kitchen

## Usage

```
PdfKitchen::Api.post({
   filename: "/var/www/html/aaa.pdf",
   access_token: "システムで発行するtoken",
   access_secret_token: "システムで発行するsecret-token",
   data: {
      text1: "aaa"
      ... 
   },
})
```

```
＊補足
フロント側にダウンロードさせたい場合のコード例
send_file(filename, :filename => "your_document.pdf", :disposition => 'inline', :type => "application/pdf")
```