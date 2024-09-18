# k8s-istio-checker
Пререквизиты:
* Для создания оператора: [kubebuilder](https://book.kubebuilder.io/quick-start.html#installation).
* Для локального запуска Kubernetes: [kind](https://kind.sigs.k8s.io/docs/user/quick-start/#installing-with-go-install), kubectl.
* Окружение: Ubuntu, Go 1.21.5.
## Для сборки проекта:
* GNU Make 4.3
# Запуск сборки
* На генерацию манифестов: make manifests
* На деплой в кубер: make install (требуется kubeconfig в **~/.kube**). ВНИМАНИЕ! Автоматически выполняется **kustomize build config/crd | kubectl apply -f -**
