# Man_ma
Manma creates the development…


<html>
<head>
    <title> ManMa's Website</title>
</head>
<body>
    <h1>Welcome to your Destiny...!</h1>

 #include <Wt/WApplication.h>
#include <Wt/WBreak.h>
#include <Wt/WContainerWidget.h>
#include <Wt/WPushButton.h>
#include <Wt/WText.h>

class BrandWebsite : public Wt::WApplication {
public:
    BrandWebsite(const Wt::WEnvironment& env) : Wt::WApplication(env) {
        setTitle("Global Heritage | Excellence & Trust");

        // Main Container (Hero Section)
        auto container = root()->addWidget(std::make_unique<Wt::WContainerWidget>());
        container->setStyleClass("hero-section");

        // Brand Title
        container->addWidget(std::make_unique<Wt::WText>("<h1>LEAD THE FUTURE</h1>"));
        container->addWidget(std::make_unique<Wt::WBreak>());

        // Subtext
        auto subtext = container->addWidget(std::make_unique<Wt::WText>(
            "<p>Inspired by a legacy of trust, we innovate for a sustainable world.</p>"
        ));

        // Call to Action Button
        auto button = container->addWidget(std::make_unique<Wt::WPushButton>("Explore Our Impact"));
        button->setMargin(20, Wt::Side::Top);
        
        // Simple styling (usually handled in an external CSS file)
        container->addStyleClass("text-center");
    }
};

int main(int argc, char **argv) {
    return Wt::WRun(argc, argv, [](const Wt::WEnvironment& env) {
        return std::make_unique<BrandWebsite>(env);
    });
}   
    

