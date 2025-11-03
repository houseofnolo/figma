// Auto layout, grids, variables, and unit scale are not yet supported
var view = UIView()
view.frame = CGRect(x: 0, y: 0, width: 375, height: 812)
view.layer.backgroundColor = UIColor(red: 1, green: 1, blue: 1, alpha: 1).cgColor

var parent = self.view!
parent.addSubview(view)
view.translatesAutoresizingMaskIntoConstraints = false
view.widthAnchor.constraint(equalToConstant: 375).isActive = true
view.heightAnchor.constraint(equalToConstant: 812).isActive = true
view.leadingAnchor.constraint(equalTo: parent.leadingAnchor, constant: 0).isActive = true
view.topAnchor.constraint(equalTo: parent.topAnchor, constant: 0).isActive = true
