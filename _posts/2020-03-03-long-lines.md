---
title: Long Lines in Rspec
description: How to split long lines in Rails RSpec
header: How to Split Long Lines in Rspec
---
It can be challenging to know where to break a long line in ruby.  Especially when writing tests in rspec.

```ruby
RSpec.describe PostHelper, :type => :helper do
  describe '#markdown' do
    it 'returns code blocks' do
      blog_text = "```ruby\nHello, World!\n```"
      expect(helper.markdown(blog_text)).to eq("<pre><code class=\"ruby\">Hello, World!\n</code></pre>\n")
    end
  end
end
```

One technique is to find the method call, `.to` in the example above, and break it there.

```ruby
RSpec.describe PostHelper, :type => :helper do
  describe '#markdown' do
    it 'returns code blocks' do
      blog_text = "```ruby\nHello, World!\n```"
      expect(helper.markdown(blog_text)).
        to eq("<pre><code class=\"ruby\">Hello, World!\n</code></pre>\n")
    end
  end
end
```

[Rubocop](https://docs.rubocop.org/en/stable/) can help improve your ruby style.  Rubocop is available as an extension in Visual Studio code.
