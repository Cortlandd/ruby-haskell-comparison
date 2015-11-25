# ruby-haskell-comparison
A side by side comparison of Ruby and Haskell syntax

    Sources:
    http://www.slideshare.net/thoughtbot/why-use-haskell
    http://tryhaskell.org

Ruby     | Haskell | Output
-------- | --------| --------
def add1(x)<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;x + 1<br />end<br />add1(5) | let &nbsp;add1 &nbsp;x = x + 1 in add1 5 | 6
"Cortland".reverse	| reverse &nbsp;"Cortland" | "dnaltroC"
"Cortland".chars.sort.join		| sort &nbsp;"Cortland" | "Cadlnort"
[42, 13, 22].sort     | sort &nbsp;[42, 13, 22] | [13, 22, 42]
puts "hi" &nbsp;; &nbsp;puts "yo" | putStrLn "hi" &nbsp;>> &nbsp;putStrLn "yo" | hi<br />yo
 a &nbsp;= &nbsp;gets<br />puts &nbsp;a|a &nbsp;<- &nbsp;getContent<br />print &nbsp;a<br /getContent >>= print|STDIN/STDOUT
 def plan_name<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;@user.account.plan.name<br />end|planName : : User -> String<br />planName = name . plan . account |
def slugs(projects)<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;projects<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;.map { IprojectI project<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;.name<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;.downcase }.uniq<br />end |slugs : : [Project] -> [String]<br />slugs = uniq .<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;map (downcase . projectName) |



